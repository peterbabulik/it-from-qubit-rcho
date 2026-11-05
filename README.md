# it-from-qubit-rcho

### The Complete Program: Inward Holographic Contraction, Topological Fault-Tolerance, and Outward Solution-Space Filtration Across Hurwitz Composition Algebras

[![Open Phase 1 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperiment.ipynb)
[![Open Phase 2 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperimentPhase2.ipynb)
[![Open Phase 3 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimentPhase3.ipynb)
[![Open Phase 4 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOexperimenPhase4.ipynb)
[![Open Phase 5 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperimentPhase5.ipynb)
[![Open Phase 5B in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RHCOeperimentPhase5b.ipynb)
[![Qiskit](https://img.shields.io/badge/Qiskit-1.x-6929C4?logo=qiskit&logoColor=white)](https://qiskit.org/)
[![Hardware](https://img.shields.io/badge/IBM_Quantum-156Q_Heron_Processors-002D9C?logo=ibm&logoColor=white)](https://quantum.ibm.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An open-source theoretical and experimental physics program establishing a self-referential **Ouroboros loop** between **Euclidean straightedge-and-compass geometry**, **Hurwitz composition algebras ($\mathbb{R}, \mathbb{C}, \mathbb{H}, \mathbb{O}$)**, **holographic entanglement entropy**, **fault-tolerant quantum computing (FTQC)**, and **asymptotic phase-space filtration**.

The complete framework has been empirically corroborated with **3,039,232 physical quantum measurements** on IBM Quantum's 156-qubit superconducting processors (`ibm_kingston`, `ibm_marrakesh`, and `ibm_fez`).

---

## 🧭 Repository Architecture

```
it-from-qubit-rcho/
├── README.md                      # Master synthesis & global benchmark report (this file)
├── phase2.md                      # Phase 2 Report: 8D Dynamics & Holonomy
├── phase3.md                      # Phase 3 Report: Topological QEC & G2/E8 Symmetries
├── phase4.md                      # Phase 4 Report: Practical FTQC & Metrology
├── phase5.md                      # Phase 5 Report: The Ouroboros Phase-Space Expansion
├── Phase5b.md                     # Phase 5B Report: Bounded Infinities & IR Vacuum Collapse
├── RCHOexperiment.ipynb           # Phase 1 Notebook: Foundational RCHO (ibm_kingston)
├── RCHOexperimentPhase2.ipynb     # Phase 2 Notebook: 4-Experiment Dynamics (ibm_marrakesh)
├── RHCOexperimentPhase3.ipynb     # Phase 3 Notebook: Fault-Tolerance & E8 (ibm_fez)
├── RHCOexperimenPhase4.ipynb      # Phase 4 Notebook: Practical FTQC & Sensing (ibm_fez/kingston)
├── RCHOexperimentPhase5.ipynb     # Phase 5 Notebook: Phase-Space Explosion (ibm_fez)
└── RHCOeperimentPhase5b.ipynb     # Phase 5B Notebook: Bounded Infinities & IR Collapse (ibm_fez)
```

---

## 🔬 Grand Master Benchmark Table Across All Phases

Theoretical predictions were verified on 156-qubit Heron processors across **3,039,232 physical measurements**:

| Phase | Core Scientific Milestone | Target QPU | Total Shots | Key Theoretical Target | **Hardware Measurement** | Status / Significance |
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
| | Scale: 154Q Full-Chip Fano-DQI | `ibm_fez` | 65,536 | 22 Parallel Blocks (154 Qubits) | **$11.19\%$** (Noise floor: $2.3\%$) | **$4.8\times$ above noise** |
| **Phase 5** | The Ouroboros Phase Expansion | `ibm_fez` | 344,064 | 8D Solution Horizon Volume $\Omega_8$ | **$3,320,878.37\times$** (MC: $\sim 691\text{k}\times$) | **$3.32\times 10^6\times$ Explosion** |
| | "Problem Defines Solution Space" | | | Dimensional Advantage ($8\text{D}$ vs $1\text{D}$) | **$527,304.2\times$** larger phase-space | Universal Horizon $R/r_0 \approx 6$ |
| **Phase 5B**| **Bounded Infinities & IR Collapse** | `ibm_fez` | 196,608 | **8D Vacuum Dilution ($L_{\max}=10^6$)** | **$0.22\%$** (1D Survival: $9.25\%$) | **$42.1\times$ 1D Localization** |
| | Nested Filtration $\mathcal{S}_{10} \subset \mathcal{S}_{10^6}$ | | | Hardware Noise Floor Observation | **Plateau at $\approx 2.2 \times 10^{-3}$** | **Vacuum Floor Proved** |
| **TOTAL** | **The Complete Research Program** | **3 QPUs** | **3,039,232** | **Full Mathematical & Physical Closure** | — | **Rigorous Convergence** |

---

## 🏛️ The Complete Ouroboros Architecture

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
                                 │   154Q Full-Chip Run      │
                                 │   3 QPUs (696k shots)     │
                                 └──────────────┬────────────┘
                                                │
                                                ▼
                                 ┌───────────────────────────┐
                                 │   PHASE 5: OUROBOROS LOOP │
                                 │ "The Problem Defines Its  │
                                 │  Own Solution Space Size" │
                                 │ Core r_0 -> Horizon R_D   │
                                 │ Omega_D = (R / r_0)^D     │
                                 │ 8D Explosion: 3.32M x     │
                                 │ ibm_fez (344k shots)      │
                                 └──────────────┬────────────┘
                                                │
                                                ▼
                                 ┌───────────────────────────┐
                                 │   PHASE 5B: INFINITY DUAL │
                                 │ Bounded Infinities        │
                                 │ S_10 ⊊ S_100 ⊊ ... ⊊ S_10^6│
                                 │ IR Vacuum Dilution Proof  │
                                 │ Hardware Noise Floor      │
                                 │ ibm_fez (197k shots)      │
                                 └───────────────────────────┘
```

---

### The Fundamental Duality: Inward Contraction vs. Outward Expansion

The entire research program resolves into a singular, self-referential duality:

1. **Inward Contraction (Phases 1–4):**  
   Partitioning an interval $r_1 = r_2 + r_3$ causes quadratic/hyper-volume to vanish from localized boundaries into the interstitial bulk:
   $$\Delta V_D = 1 - \left(x^D + (1-x)^D\right)$$
   This missing content manifests physically as **holographic entanglement entropy**, which provides the topological code space for **quantum error correction (QEC)** and fault-tolerant computation.
2. **Outward Expansion (Phase 5):**  
   Stochastically probing outward beyond an initial problem constraint ($L_i = r_0 + \Delta L$ with $\Delta L > 0$) causes discrete probing rays to condense into an asymptotic **Solution Horizon ($R_D$)**.
   The hyper-volume of accessible answers explodes under the power of the Hurwitz dimensions:
   $$\Omega_D = \frac{V_D(R_D)}{V_D(r_0)} = \left(\frac{R_D}{r_0}\right)^D$$
3. **The Ouroboros Closure & The Size of Solution Space:**  
   **The problem itself defines the size of its own solution space.** The initial question ($r_0$) dictates the asymptotic curvature and volume of the manifold of its possible answers ($R_D$), with the 8D octonionic manifold expanding to **$3,320,878\times$ the volume of the problem core** on physical hardware.
4. **Bounded Infinities & The Infrared Cutoff (Phase 5B):**  
   Larger infinities strictly contain smaller infinities ($\mathcal{S}_{10} \subsetneq \dots \subsetneq \mathcal{S}_{10^6}$), but dilute the core density as $10^{-D \cdot k}$. If $L_{\max} \to \infty$, core information vanishes to measure zero. Thus, **every physically solvable problem requires an upper cutoff ($L_{\max}$)** to remain observable above the zero-point vacuum noise floor.

---

## 🔬 Phase-by-Phase Technical Overview

### Phase 1: Foundations of Geometric Holography (RCHO)
* **Notebook:** [`RCHOexperiment.ipynb`](./RCHOexperiment.ipynb) | **Hardware:** `ibm_kingston` (344,064 shots)
* **Core Discovery:** Proved that the classical area deficit $\Delta S = 2\pi r_2 r_3 = 2x(1-x)S_1$ is identical to the **linear entanglement entropy** of a bipartite state: $S_L = 1 - \text{Tr}(\rho_A^2) = 2x(1-x)$. Power-norm scaling across Hurwitz algebras ($\mathbb{R}, \mathbb{C}, \mathbb{H}, \mathbb{O}$) was verified with **$0.001\%$ accuracy** on physical superconducting qubits.

### Phase 2: Advanced 8D Dynamics, Holonomy, and Multi-Slider Geometry
* **Technical Report:** [`phase2.md`](./phase2.md) | **Notebook:** [`RCHOexperimentPhase2.ipynb`](./RCHOexperimentPhase2.ipynb) | **Hardware:** `ibm_marrakesh` (1,064,960 shots)
* **Core Discovery:** 
  1. *Fano Associator Witness:* Detected non-associative phase frustration ($>9.0\%$ contrast) away from the isotropic midpoint.
  2. *8D Okteract Quantum Walk:* Tracked wave packet dispersion across 256 vertices and 1024 edges, hitting the equatorial plane ($d = 3.920 \approx 4.000$) with a spreading entropy of $7.226$ bits.
  3. *Dynamic Berry Holonomy:* Proved moving the slider accumulates a topological gauge field, reconstructing a $+59.92^\circ \to -60.31^\circ$ phase with a nodal zero-crossing at $x=0.50$.
  4. *Ternary Arbelos:* Trisection of the line peaked at $66.621\%$ (theory: $66.667\%$), with 8D octonionic absorption reaching $99.952\%$.

### Phase 3: Fault-Tolerant Architectures, $G_2$ Automorphism, and the $E_8$ Root Lattice
* **Technical Report:** [`phase3.md`](./phase3.md) | **Notebook:** [`RHCOexperimentPhase3.ipynb`](./RHCOexperimentPhase3.ipynb) | **Hardware:** `ibm_fez` (393,216 shots)
* **Core Discovery:**
  1. *Fano QEC (Steane $[[7, 1, 3]]$):* Restored bit-flip ($X$) errors from $1.75\%$ to $88.26\%$.
  2. *Advanced QECD:* Restored phase-flip ($Z$) errors from $1.90\%$ to $88.31\%$ and protected a continuous geometric slider at $86.80\%$ fidelity under persistent physical destruction.
  3. *Lie Group $G_2$ on $E_8$ Roots:* Prepared the 240 integral octonions forming the $E_8$ root lattice, demonstrating automorphism invariance with a stability score of $98.66 / 100.00\%$.

### Phase 4: Practical Applications of Quantum Error Correction (FTQC) & Full-Chip Scale
* **Technical Report:** [`phase4.md`](./phase4.md) | **Notebook:** [`RHCOexperimenPhase4.ipynb`](./RHCOexperimenPhase4.ipynb) | **Hardware:** `ibm_fez`, `ibm_kingston`, `ibm_marrakesh` (696,320 shots)
* **Core Discovery:**
  1. *Transversal Clifford Gates ($H_L, S_L$):* Reconstructed the 6-pole Logical Bloch Sphere with $93.06\%$ fidelity; neutralized mid-circuit faults with $0.44\%$ deviation (zero error cascading).
  2. *14-Qubit Transversal $\text{CNOT}_L$:* Synthesized the Logical Bell State $|\Phi^+\rangle_L$, boosting fidelity from sub-classical $46.07\%$ to **$72.83\%$**, breaking the $50\%$ classical limit.
  3. *Quantum Memory & Pseudo-Threshold:* Mapped memory retention under dephasing noise, confirming the fault-tolerance threshold at $p_{\mathrm{th}} \approx 8.0\%$.
  4. *Protected Metrology:* Fano QEC restored blinded sensor visibility from $1.25\%$ to **$90.21\%$** ($+88.96\%$ SNR gain).
  5. *154-Qubit Scale Run:* Ran 22 parallel Fano-DQI blocks across $98.7\%$ of `ibm_fez` simultaneously, maintaining constructive interference $4.8\times$ above the uniform noise floor.

### Phase 5: The Ouroboros Phase-Space Expansion
* **Technical Report:** [`phase5.md`](./phase5.md) | **Notebook:** [`RCHOexperimentPhase5.ipynb`](./RCHOexperimentPhase5.ipynb) | **Hardware:** `ibm_fez` (344,064 shots)
* **Core Discovery:**
  1. *The Problem Defines Its Own Solution Space:* A bounded problem core ($r_0$) radiating probing trajectories defines a solution horizon ($R_D$) whose volume ratio scales as $(R/r_0)^D$.
  2. *EVT Stabilization:* Verified that horizon radius stabilizes logarithmically ($R/r_0 \approx 6.0 - 6.5$) via Gumbel Extreme Value Theory.
  3. *The $3.32\times 10^6\times$ Octonionic Explosion:* Hardware measurements on `ibm_fez` confirmed that while 1D scales as $6.30\times$ and 2D as $39.20\times$, the 8D octonionic manifold undergoes a **$3,320,878.37\times$ phase-space explosion**, yielding a **$527,304\times$ dimensional advantage** over 1D systems.

### Phase 5B: Bounded Infinities, Nested Filtration, and the Infrared Vacuum Collapse
* **Technical Report:** [`Phase5b.md`](./Phase5b.md) | **Notebook:** [`RHCOeperimentPhase5b.ipynb`](./RHCOeperimentPhase5b.ipynb) | **Hardware:** `ibm_fez` (196,608 shots)
* **Core Discovery:**
  1. *Nested Filtration of Infinities:* Demonstrated that larger solution spaces strictly enclose smaller cutoffs ($\mathcal{S}_{10} \subsetneq \dots \subsetneq \mathcal{S}_{10^6}$), expanding the solution volume by $10^{D \cdot k}$ up to $10^{48}\times$ in 8D.
  2. *Infrared Catastrophe Proof:* As cutoff scale expands to $10^6$, 8D core information density collapses down to $0.22\%$, displaying **$42.1\times$ higher localization in 1D** and proving that physically solvable problems require an upper boundary horizon.
  3. *Observation of the Vacuum Noise Floor:* Showed that on real quantum hardware, dilution plateaus at the physical zero-point noise floor ($\approx 2.2 \times 10^{-3}$), demonstrating where continuous mathematical dilution dissolves into the physical quantum vacuum.

---

## 💻 Quickstart & Reproduction

### Google Colab One-Click Execution
* **Phase 1 Benchmark (RCHO Core):** [![Open Phase 1 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperiment.ipynb)
* **Phase 2 Advanced (8D Dynamics & Holonomy):** [![Open Phase 2 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peterbabulik/it-from-qubit-rcho/blob/main/RCHOexperimentPhase2.ipynb)
* **Phase 3 Fault-Tolerance (Steane QEC & G2/E8):** [![Open Phase 3 in Colab](https://colab.research.
