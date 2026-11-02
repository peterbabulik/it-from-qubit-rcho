# Phase 3: Fault-Tolerant Architectures, Octonionic Automorphisms ($G_2$), and the $E_8$ Root Lattice on Quantum Hardware

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimentPhase3.ipynb)
[![Qiskit](https://img.shields.io/badge/Qiskit-1.x-6929C4?logo=qiskit&logoColor=white)](https://qiskit.org/)
[![Hardware](https://img.shields.io/badge/IBM_Quantum-ibm__fez_(156Q)-002D9C?logo=ibm&logoColor=white)](https://quantum.ibm.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This phase concludes the experimental arc by demonstrating the operational and physical applications of the **RCHO framework**:
1. **Fault-Tolerant Quantum Error Correction (QEC) on the Fano Plane:** Using the 7 points and 7 lines of $PG(2, \mathbb{F}_2)$ to implement the Calderbank-Shor-Steane $[[7, 1, 3]]$ code, demonstrating simultaneous protection against bit-flip ($X$) and phase-flip ($Z$) errors, as well as protecting a continuous geometric slider state under active physical destruction.
2. **The Exceptional Lie Group $G_2$ and the $E_8$ Root Lattice:** Preparing an 8-qubit representation of the 240 roots of the $E_8$ lattice and proving the invariant stability of the octonionic automorphism group $G_2 = \text{Aut}(\mathbb{O})$ on quantum hardware.

The complete code and hardware execution workflows are available in [`RHCOexperimentPhase3.ipynb`](./RHCOexperimentPhase3.ipynb).

---

## 📊 Summary of Phase 3 Hardware Benchmark Results

A total of **393,216 physical quantum measurements** were executed on the 156-qubit Heron processor `ibm_fez`:

| Experiment | Qubits | Total Shots | Core Performance Metric | Theoretical Target | **Measured on `ibm_fez`** | Status |
| :--- | :---: | :---: | :--- | :---: | :---: | :---: |
| **Exp 1: Fano QEC ($X$-Errors)** | 7 | 65,536 | Mean Error Detection Accuracy | $100.00\%$ | **$82.66\%$** | Validated |
| | | | Raw State Fidelity under Error | $0.00\%$ | **$1.75\%$** | Collapsed |
| | | | Fano Corrected State Fidelity | $100.00\%$ | **$88.26\%$** | **Recovered!** |
| **Exp 1B: Advanced QECD ($Z$-Errors)**| 7 | 155,648 | Raw Phase Fidelity under $Z$-Error | $0.00\%$ | **$1.90\%$** | Collapsed |
| | | | Fano Corrected Phase Fidelity | $100.00\%$ | **$88.31\%$** | **Recovered!** |
| | | | Protected Continuous Slider Fidelity | $100.00\%$ | **$86.80\%$** | **Protected!** |
| **Exp 2: Lie Group $G_2$ & $E_8$** | 8 | 172,032 | $E_8$ Parity Subspace Fidelity | $50.00\%$ | **$49.64\%$** | **$\pm 0.36\%$ Error** |
| | | | $G_2$ Automorphism Stability Score | $100.00\%$ | **$98.66\%$** | **Confirmed** |
| | | | Invariance Fluctuation ($\sigma$) | $0.00\%$ | **$\pm 1.34\%$** | Minimal |

---

## 🔬 Detailed Experimental Breakdown

### Experiment 1 & 1B: Quantum Error Correction on the Fano Plane (The Steane $[[7, 1, 3]]$ Code)
* **Hardware Target:** `ibm_fez` (Job IDs: `dbkdqagnceqs73allvh0` and `dbkdsgpkdqps73928efg`)
* **Execution:** 8 circuits $\times$ 8,192 shots + 19 circuits $\times$ 8,192 shots = **221,184 total measurements**
* **Theoretical Mapping:**  
  The 7 points of the Fano plane represent the 7 physical qubits of the Steane code. The 7 lines of the Fano plane define the syndrome check relations:
  $$s_1 = q_3 \oplus q_4 \oplus q_5 \oplus q_6, \quad s_2 = q_1 \oplus q_2 \oplus q_5 \oplus q_6, \quad s_3 = q_0 \oplus q_2 \oplus q_4 \oplus q_6$$
  The 7 non-zero syndrome integers in $\mathbb{F}_2^3$ map 1-to-1 to the 7 points of the Fano plane, with collinear points satisfying $s_i \oplus s_j \oplus s_k = (0, 0, 0)$.

#### 1. Bit-Flip ($X$) Detection and Recovery (Exp 1)
* **Syndrome Matrix:** Evaluated across the 8 test cases $\{I, X_0, \dots, X_6\}$. The processor identified the faulty qubit with an average diagonal detection accuracy of **$82.66\%$**.
* **Active Recovery:** Single-qubit errors collapsed the raw fidelity of the logical zero state $|\bar{0}\rangle$ to **$1.75\%$**. The Fano decoder dynamically located the faulty vertex and flipped it back, restoring the logical state fidelity to **$88.26\%$** (peaking at $91.2\%$).

```
======================================================================
PHASE 3, EXP 1 REPORT: FANO QEC PERFORMANCE ON ibm_fez
Total Execution Shots: 65,536 shots
----------------------------------------------------------------------
  Unperturbed Baseline Fidelity:           93.41%
  Average Raw Fidelity during Errors:       1.75% (Collapsed)
  Average Recovered Fidelity after QEC:    88.26% (Restored!)
  Average Error Detection Accuracy:        82.66%
======================================================================
```

#### 2. Advanced QECD: Dual Phase-Flip ($Z$) and Continuous Slider Protection (Exp 1B)
* **Phase-Flip ($Z$) Correction:** In the dual Hadamard basis $|\bar{+}\rangle$, physical phase errors $Z_0$ through $Z_6$ collapsed raw coherence to **$1.90\%$**. The CSS Fano parity decoder recovered the logical state to **$88.31\%$** (clean baseline at **$97.66\%$**).
* **Fault-Tolerant Geometric Slider:** An arbitrary continuous superposition $|\bar{\psi}(x)\rangle = \sqrt{x}|\bar{0}\rangle + \sqrt{1-x}|\bar{1}\rangle$ was encoded into the 7-qubit manifold while subjecting the central Fano hub ($q_3$) to persistent $100\%$ physical destruction. While raw fidelity collapsed to **$0.63\%$**, the active Fano decoder maintained the slider space protected at **$86.80\%$** across all coordinates $x \in [0, 1]$.

```
======================================================================
ADVANCED QECD EVALUATION REPORT ON ibm_fez
----------------------------------------------------------------------
  Test A: Phase-Flip Z Baseline:                97.66%
  Test A: Mean Damaged Phase Fidelity:           1.90%
  Test A: Mean Corrected Phase Fidelity:        88.31% (Fully Recovered!)
----------------------------------------------------------------------
  Test B: Mean Damaged Slider Fidelity:          0.63%
  Test B: Mean Protected Slider Fidelity:        86.80% (Protected!)
======================================================================
```

---

### Experiment 2: The Exceptional Lie Group $G_2$ and the $E_8$ Root Lattice
* **Hardware Target:** `ibm_fez` (Job ID: `dbkdujt6p51s73cmeel0`)
* **Execution:** 21 circuits $\times$ 8,192 shots = **172,032 total measurements (8 physical qubits)**
* **Theoretical Mapping:**  
  * The exceptional Lie group $G_2 = \text{Aut}(\mathbb{O})$ is the 14-dimensional automorphism group preserving the octonionic multiplication table and Fano plane orientation.
  * In 8-dimensional space $\mathbb{R}^8 \cong \mathbb{O}$, the root system of the exceptional Lie algebra $\mathfrak{e}_8$ consists of **240 roots** (112 integer roots from the $D_8$ lattice and 128 half-integer spinor roots of even parity).
  * The 240 roots of $E_8$ are identical to the **240 unit Cayley integral octonions**.

#### Hardware Verification:
* An 8-qubit register was prepared in the $E_8$ root projection state and driven through a continuous $2\pi$ rotation via the $G_2$ Lie algebra generator $\exp(i\phi \mathfrak{g}_2)$ spanning interlocking Fano triads.
* **$E_8$ Parity Subspace Level:** The measured mean invariant level was **$49.64\%$**, matching the theoretical 128-state parity subspace of $256$ states ($50.00\%$) with an error of only **$\pm 0.36\%$**.
* **$G_2$ Automorphism Stability:** Across the entire $2\pi$ parameter sweep, the standard deviation remained tightly bounded at **$\pm 1.34\%$**, yielding a $G_2$ stability score of **$98.66 / 100.00\%$**.
* **Harmonic Symmetry:** Deviations from the baseline exhibited symmetric $60^\circ$ periodicity, directly reflecting the hexagonal root geometry of the $G_2$ Lie algebra.

```
======================================================================
PHASE 3, EXP 2 REPORT: G2 AUTOMORPHISM & E8 LATTICE ON ibm_fez
Total Execution Shots: 172,032 shots (8 Qubits)
----------------------------------------------------------------------
  Mean E8 Root Lattice Fidelity:     49.64% (Theory: 50.00%)
  G2 Invariance Fluctuation (Std):    1.34%
  G2 Automorphism Stability Score:   98.66 / 100.00%
  Symmetry Preservation:             CONFIRMED (Zero structural collapse across 2*pi)
======================================================================
```

---

## 🛠️ Reproduction & Verification

To execute the Phase 3 notebook or reproduce the analysis locally:

```bash
# Clone the repository
git clone https://github.com/peterbabulik/it-from-qubit-rcho.git
cd it-from-qubit-rcho

# Install required dependencies
pip install qiskit qiskit-ibm-runtime matplotlib numpy
```

Open and run [`RHCOexperimentPhase3.ipynb`](./RHCOexperimentPhase3.ipynb) in Google Colab or your local Jupyter environment.

---

## 📜 References

1. **Steane, A. M.** (1996). *Error Detecting Codes in Quantum Theory.* Physical Review Letters, 77(5), 793–797.
2. **Calderbank, A. R., & Shor, P. W.** (1996). *Good quantum error-correcting codes exist.* Physical Review A, 54(2), 1098.
3. **Baez, J. C.** (2002). *The Octonions.* Bulletin of the American Mathematical Society, 39(2), 145–205.
4. **Conway, J. H., & Smith, D. A.** (2003). *On Quaternions and Octonions: Their Geometry, Arithmetic, and Symmetry.* A K Peters/CRC Press.
5. **Furey, C.** (2018). *Three generations, two unbroken gauge symmetries, and one eight-dimensional algebra.* Physics Letters B, 785, 84–89.
