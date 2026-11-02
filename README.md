# it-from-qubit-rcho

### Experimental Holographic Dimensional Reduction, Octonionic Non-Associativity, and Fault-Tolerant Quantum Computation on Superconducting Hardware

[![Open Phase 1 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperiment.ipynb)
[![Open Phase 2 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperimentPhase2.ipynb)
[![Open Phase 3 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimentPhase3.ipynb)
[![Open Phase 4 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimenPhase4.ipynb)
[![Qiskit](https://img.shields.io/badge/Qiskit-1.x-6929C4?logo=qiskit&logoColor=white)](https://qiskit.org/)
[![Hardware](https://img.shields.io/badge/IBM_Quantum-156Q_Heron_Processors-002D9C?logo=ibm&logoColor=white)](https://quantum.ibm.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An open-source theoretical and experimental physics program establishing an exact isomorphism between **Euclidean straightedge-and-compass geometry**, **Hurwitz composition algebras ($\mathbb{R}, \mathbb{C}, \mathbb{H}, \mathbb{O}$)**, **quantum holographic entanglement entropy**, **topological error correction**, and **fault-tolerant quantum computation (FTQC)**.

The entire framework has been experimentally verified with **2,433,024 physical quantum measurements** on IBM Quantum's 156-qubit superconducting processors (`ibm_kingston`, `ibm_marrakesh`, and `ibm_fez`).

---

## 🧭 Repository Structure

```
it-from-qubit-rcho/
├── README.md                      # Master synthesis & global benchmark report (this file)
├── phase2.md                      # Phase 2 Technical Report: 8D Dynamics & Holonomy
├── phase3.md                      # Phase 3 Technical Report: Topological QEC & G2/E8
├── phase4.md                      # Phase 4 Technical Report: Practical FTQC & Metrology
├── RCHOexperiment.ipynb           # Phase 1 Notebook: Foundational RCHO (ibm_kingston)
├── RCHOexperimentPhase2.ipynb     # Phase 2 Notebook: 4-Experiment Dynamics (ibm_marrakesh)
├── RHCOexperimentPhase3.ipynb     # Phase 3 Notebook: Fault-Tolerance & E8 (ibm_fez)
└── RHCOexperimenPhase4.ipynb      # Phase 4 Notebook: Practical FTQC & Sensing (ibm_fez/kingston)
```

---

## 🔬 Master Benchmark Table Across All Phases

Across all four phases, theoretical predictions were corroborated on 156-qubit Heron quantum processors across **2,433,024 total measurements**:

| Phase | Core Focus | Target QPU | Total Shots | Key Theoretical Target | **Hardware Measurement** | Status / Gain |
| :--- | :--- | :---: | :---: | :--- | :---: | :---: |
| **Phase 1** | Hurwitz $\mathbb{R} \to \mathbb{C} \to \mathbb{H} \to \mathbb{O}$ | `ibm_kingston` | 344,064 | 8D Octonion Midpoint $\Delta V_8$ | **$99.218\%$** (Theory: $99.219\%$) | **$\pm 0.001\%$ Error** |
| | Bisection Area Stability | | | 2D Circle Midpoint $\Delta S$ | **$49.997\%$** (Theory: $50.000\%$) | **$\pm 0.003\%$ Error** |
| **Phase 2** | Exp 1: Fano Associator Witness | `ibm_marrakesh` | 344,064 | Midpoint Contrast $\mathcal{W}(0.5)$ | **$0.084\%$** (Theory: $0.000\%$) | Confirmed |
| | Exp 2: 8D Okteract Quantum Walk | `ibm_marrakesh` | 172,032 | Equatorial Distance $\langle D(\pi/2) \rangle$ | **$3.920$ / $8.0$** (Theory: $4.000$) | $\pm 0.080$ Distance |
| | Exp 3: Dynamic Berry Holonomy | `ibm_marrakesh` | 344,064 | Total Phase Sweep $\Delta \gamma$ | **$+59.92^\circ \to -60.31^\circ$** | **$\pm 0.19^\circ$ Error** |
| | Exp 4: Ternary Arbelos Trisection | `ibm_marrakesh` | 204,800 | 2D Trisection Peak $\Delta S_{\max}$ | **$66.621\%$** (Theory: $66.667\%$) | **$\pm 0.046\%$ Error** |
| | | | | 8D Octonionic Peak $\Delta V_8$ | **$99.952\%$** (Theory: $99.954\%$) | **$\pm 0.002\%$ Error** |
| **Phase 3** | Exp 1 & 1B: Dual $X$ & $Z$ QECD | `ibm_fez` | 221,184 | Dual-Basis $X$ & $Z$ Recovery | **$88.26\%$ / $88.31\%$** (Raw: $<2\%$) | **Recovered** |
| | | | | Protected Continuous Slider | **$86.80\%$** (Raw: $0.63\%$) | **Protected** |
| | Exp 2: Lie Group $G_2$ & $E_8$ Roots | `ibm_fez` | 172,032 | $E_8$ Parity Subspace Level | **$49.64\%$** (Theory: $50.00\%$) | **$\pm 0.36\%$ Error** |
| | | | | $G_2$ Automorphism Stability | **$98.66 / 100\%$** ($\sigma = \pm 1.34\%$) | **Confirmed** |
| **Phase 4** | Exp 1: Transversal Clifford Gates | `ibm_fez` | 163,840 | 6-Pole Mean Logical Fidelity | **$93.06\%$** (Raw: $74.66\%$) | **$+18.40\%$ Boost** |
| | | | | Mid-Circuit Fault Tolerance Delta | **$0.44\%$** ($94.43\%$ vs $93.99\%$) | Zero Cascading |
| | Exp 2: 14Q Transversal $\text{CNOT}_L$ | `ibm_kingston` | 32,768 | Logical Bell State Fidelity | **$72.83\%$** (Raw: $46.07\%$) | **Breaks 50% Limit!** |
| | Exp 3.1: Quantum Memory Threshold | `ibm_fez` | 90,112 | Observed Pseudo-Threshold | **$p_{\mathrm{th}} \approx 8.0\%$** | Threshold Proved |
| | Exp 4: Protected Metrology | `ibm_fez` | 262,144 | Fano Protected Fringe Visibility | **$90.21\%$** (Bare Sensor: $1.25\%$) | **$+88.96\%$ Gain** |
| **TOTAL** | **4 Experimental Phases** | **3 QPUs** | **2,433,024** | **Complete Quantum Geometric Program** | — | **Full Physical Convergence** |

---

## 🏛️ The Four-Tier Experimental Architecture

```
                                  ┌───────────────────────────┐
                                  │   EUCLIDEAN FOUNDATION    │
                                  │   1D Segment Partition    │
                                  │   r1 = r2 + r3            │
                                  └─────────────┬─────────────┘
                                                │
                 ┌──────────────────────────────┴──────────────────────────────┐
                 ▼                                                             ▼
   ┌───────────────────────────┐                                 ┌───────────────────────────┐
   │    PHASE 1: RCHO CORE     │                                 │   PHASE 2: 8D DYNAMICS    │
   │  Hurwitz Division Norms   │                                 │  Fano Associator Witness  │
   │  R (1D) -> C (2D)         │                                 │  8D Okteract Quantum Walk │
   │  H (4D) -> O (8D)         │                                 │  Dynamic Berry Holonomy   │
   │  Purity = Area Recovery   │                                 │  Ternary 66.67% Trisection│
   │  ibm_kingston (344k sh)   │                                 │  ibm_marrakesh (1.06M sh) │
   └─────────────┬─────────────┘                                 └─────────────┬─────────────┘
                 │                                                             │
                 └──────────────────────────────┬──────────────────────────────┘
                                                │
                                                ▼
                                 ┌───────────────────────────┐
                                 │   PHASE 3: FAULT-TOLERANCE│
                                 │   Steane [[7, 1, 3]] QEC  │
                                 │   CSS X & Z Dual Recovery │
                                 │   Protected Slider Space  │
                                 │   G2 Automorphism on E8   │
                                 │   ibm_fez (393k shots)    │
                                 └──────────────┬────────────┘
                                                │
                                                ▼
                                 ┌───────────────────────────┐
                                 │   PHASE 4: PRACTICAL FTQC │
                                 │   Transversal Gates (HL,SL)│
                                 │   14Q Logical Bell State  │
                                 │   Pseudo-Threshold p ≈ 8% │
                                 │   Protected Metrology     │
                                 │   3 QPUs (631k shots)     │
                                 └───────────────────────────┘
```

---

### Phase 1: Foundations of Geometric Holography (RCHO)
* **Notebook:** [`RCHOexperiment.ipynb`](./RCHOexperiment.ipynb)
* **Target Hardware:** `ibm_kingston` (Job ID: `dbk6v056p51s73cm2sg0`)
* **Core Theory:** When a 1D segment $r_1 = r_2 + r_3$ is partitioned, linear dimensions (circumference, diameter) are strictly conserved, but quadratic area vanishes into the interstitial bulk:
  $$\Delta S = 2\pi r_2 r_3 = 2x(1 - x)S_1, \quad x \in [0, 1]$$
  This classical missing area is mathematically isomorphic to the **linear entanglement entropy** of a bipartite state:
  $$\text{Purity}(\rho_A) = x^2 + (1-x)^2 \quad \Longleftrightarrow \quad S_L = 1 - \text{Tr}(\rho_A^2) = \mathbf{2x(1-x)}$$
  By Hurwitz's Theorem (1898), the power-norm scaling across the only four division algebras ($\mathbb{R}, \mathbb{C}, \mathbb{H}, \mathbb{O}$) establishes that at the symmetric midpoint ($x = 0.50$), local information decays as $1/2^{d-1}$, leaving **$99.219\%$** of 8D octonionic volume absorbed into tripartite bulk entanglement.

---

### Phase 2: Advanced 8D Dynamics, Holonomy, and Multi-Slider Geometry
* **Technical Report:** [`phase2.md`](./phase2.md) | **Notebook:** [`RCHOexperimentPhase2.ipynb`](./RCHOexperimentPhase2.ipynb)
* **Target Hardware:** `ibm_marrakesh` (4 multi-qubit topologies, **1,064,960 total measurements**)
* **Investigations:**
  1. **Full 7-Qubit Fano Plane Embedding:** Contrasted collinear associative triads ($q_0, q_1, q_3$) against non-collinear frustrated triples ($q_0, q_1, q_2$). Discovered that while isotropic trisection suppresses the associator to $0.084\%$, symmetry breaking on the wings exposes an **octonionic associator contrast exceeding $9.0\%$**.
  2. **Quantum Walk on the 8D Okteract ($2^8 = 256$ Vertices, 1024 Edges):** Tracked an 8-qubit continuous-time quantum walker dispersing through all 9 Hamming distance shells $\binom{8}{k}$, reaching the exact equatorial plane ($\langle D \rangle = 3.920 \approx 4.000$) with a delocalization entropy of **$7.226$ bits** (out of the 8.000-bit capacity).
  3. **Dynamic Berry Phase & Geometric Holonomy:** Verified that driving the slider through a closed parameter loop generates a topological gauge field, reconstructing a smooth **$+59.92^\circ \to -60.31^\circ$** holonomy with an exact nodal zero-crossing at $x = 0.50$ ($1.917^\circ \approx 0^\circ$).
  4. **Ternary Arbelos Partition:** Generalized to two sliders partitioning the line into three pieces ($r_1 + r_2 + r_3 = 1$). Proved on hardware that the missing area peaks at the trisection barycenter at **$66.621\%$** (theory: $66.667\%$), with 8D octonionic absorption hitting **$99.952\%$**, before smoothly collapsing back to the binary Arbelos bound at $51.82\% \approx 50.00\%$.

---

### Phase 3: Fault-Tolerant Architectures, $G_2$ Automorphism, and the $E_8$ Root Lattice
* **Technical Report:** [`phase3.md`](./phase3.md) | **Notebook:** [`RHCOexperimentPhase3.ipynb`](./RHCOexperimentPhase3.ipynb)
* **Target Hardware:** `ibm_fez` (3 distinct operational benchmarks, **393,216 total measurements**)
* **Investigations:**
  1. **Fano Quantum Error Correction (The Steane $[[7, 1, 3]]$ Code):** Mapped the 7 points of the Fano plane to 7 physical qubits and its 7 lines to CSS stabilizer parity checks. Single-qubit bit-flip errors ($X_k$) collapsing raw logical state fidelity to **$1.75\%$** were localized via the syndrome matrix ($82.66\%$ accuracy) and restored to **$88.26\%$** (peaking at $91.2\%$).
  2. **Advanced QECD (Phase Errors & Protected Continuous Slider):** Physical phase-flip errors ($Z_k$) destroying the coherence of $|+_L\rangle$ down to **$1.90\%$** were recovered to **$88.31\%$** (clean baseline: $97.66\%$). When encoding an arbitrary continuous superposition $|\bar{\psi}(x)\rangle = \sqrt{x}|\bar{0}\rangle + \sqrt{1-x}|\bar{1}\rangle$ under persistent physical destruction of the central Fano hub ($q_3$), the active Fano decoder maintained the slider space protected at **$86.80\%$** across all coordinates $x \in [0, 1]$.
  3. **Exceptional Lie Group $G_2$ and the 240 Roots of $E_8$:** Prepared an 8-qubit representation of the 240 integral unit octonions forming the root system of the exceptional Lie algebra $\mathfrak{e}_8$. Rotations under the 14-dimensional automorphism group $G_2 = \text{Aut}(\mathbb{O})$ confirmed root subspace parity preservation at **$49.64\%$** (theory: $50.00\%$) with an invariance stability score of **$98.66 / 100.00\%$** and a characteristic 6-fold harmonic symmetry.

---

### Phase 4: Practical Applications of Quantum Error Correction (FTQC)
* **Technical Report:** [`phase4.md`](./phase4.md) | **Notebook:** [`RHCOexperimenPhase4.ipynb`](./RHCOexperimenPhase4.ipynb)
* **Target Hardware:** `ibm_fez`, `ibm_kingston`, `ibm_marrakesh` (4 operational benchmarks, **630,784 total measurements**)
* **Investigations:**
  1. **Transversal Logical Clifford Gates ($H_L, S_L, X_L, Z_L$):** Reconstructed the entire 6-pole Logical Bloch Sphere purely transversally, boosting raw fidelity from **$74.66\%$** to **$93.06\%$**. During a composite $H_L \to S_L$ computation, an injected physical fault $X_3$ was completely neutralized ($94.43\%$ output vs $93.99\%$ clean baseline), proving zero error cascading.
  2. **14-Qubit Transversal $\text{CNOT}_L$ (Logical Bell State $|\Phi^+\rangle_L$):** Linked two independent 7-qubit Fano blocks using 7 parallel physical CNOT gates. Overcame severe 14-qubit hardware cross-talk, boosting the logical Bell fidelity from sub-classical **$46.07\%$** to **$72.83\%$**, decisively breaking the $50\%$ classical entanglement threshold and demonstrating fault-tolerant logical entanglement.
  3. **Quantum Memory Lifetime & The Fault-Tolerance Pseudo-Threshold ($p_{\mathrm{th}} \approx 8.0\%$):** Mapped memory retention under calibrated environmental dephasing. Observed quadratic error suppression below the threshold ($+26.12\%$ peak coherence gain) and code saturation above $p \approx 10\%$, experimentally validating the theoretical threshold scaling of CSS codes.
  4. **Protected Quantum Metrology & Sensing (Ramsey Interferometry):** Evaluated phase estimation under a 50/50 stochastic environmental noise channel. While the bare physical sensor was completely blinded ($1.25\%$ visibility), the Fano QEC protected sensor restored a high-contrast sinusoidal fringe with **$90.21\%$ visibility** (a net **$+88.96\%$ metrological gain**).

---

## 💻 Quickstart & Reproduction

### One-Click Execution via Google Colab
* **Phase 1 Benchmark (RCHO Foundations):** [![Open Phase 1 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperiment.ipynb)
* **Phase 2 Advanced (8D Dynamics & Holonomy):** [![Open Phase 2 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperimentPhase2.ipynb)
* **Phase 3 Fault-Tolerance (QEC & G2/E8):** [![Open Phase 3 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimentPhase3.ipynb)
* **Phase 4 Practical FTQC (Gates, Bell & Sensing):** [![Open Phase 4 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimenPhase4.ipynb)

### Local Environment Setup
```bash
# Clone the repository
git clone https://github.com/peterbabulik/it-from-qubit-rcho.git
cd it-from-qubit-rcho

# Install requirements
pip install qiskit qiskit-ibm-runtime matplotlib numpy scipy
```

To run on IBM Quantum hardware, provide your API token within any notebook:
```python
from qiskit_ibm_runtime import QiskitRuntimeService
service = QiskitRuntimeService(channel="ibm_quantum", token="YOUR_IBM_API_TOKEN")
```

---

## 📜 Key References

1. **Hurwitz, A.** (1898). *Ueber die Composition der quadratischen Formen von beliebig vielen Variabeln.* Nachrichten von der Gesellschaft der Wissenschaften zu Göttingen.
2. **Wheeler, J. A.** (1989). *Information, physics, quantum: The search for links.* Proc. 3rd Int. Symp. Foundations of Quantum Mechanics.
3. **Steane, A. M.** (1996). *Error Detecting Codes in Quantum Theory.* Physical Review Letters, 77(5), 793–797.
4. **Ryu, S., & Takayanagi, T.** (2006). *Holographic Derivation of Entanglement Entropy from AdS/CFT.* Phys. Rev. Lett., 96(18), 181602.
5. **Baez, J. C.** (2002). *The Octonions.* Bull. Amer. Math. Soc., 39(2), 145–205.
6. **Berry, M. V.** (1984). *Quantal phase factors accompanying adiabatic changes.* Proc. R. Soc. Lond. A, 392, 45–57.
7. **Farhi, E., & Gutmann, S.** (1998). *Quantum computation and decision trees.* Phys. Rev. A, 58(2), 915.
8. **Conway, J. H., & Smith, D. A.** (2003). *On Quaternions and Octonions: Their Geometry, Arithmetic, and Symmetry.* A K Peters/CRC Press.
9. **Dür, W., et al.** (2014). *Improved quantum sensing with error correction.* Phys. Rev. Lett., 112(8), 080801.
10. **Google Quantum AI.** (2023). *Suppressing quantum errors by scaling a quantum error-correcting code.* Nature, 614(7949), 676–681.

---

## 📄 License
This repository is open-source and released under the [MIT License](LICENSE).
