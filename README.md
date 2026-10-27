## 🎓 Master's Thesis

**Title:** Vacuum Decay in the Semiclassical and Stochastic Approaches

**Institution:** University of Göttingen, Germany  
**Supervisor:** Prof. Laura Covi  
**Second Examiner:** Prof. Jens Niemeyer

This repository contains the original numerical implementations developed for the master's thesis. The code is preserved in its original form to maintain consistency with the calculations and results presented in the thesis.

# semi-classical-and-stochastic-comparison-thesis

A comprehensive numerical framework for studying vacuum decay, comparing **Semi-Classical (Coleman)** methodologies with the **Stochastic Framework**. This research investigates phase transitions in contexts ranging from flat spacetime to gravity-inclusive models (thin-wall approximation) and from 1D scalar fields to 2D coupled systems.

---

## 📋 Project Overview
This repository contains the numerical implementations used to analyze vacuum decay through two primary lenses:
*   **Semi-Classical Case:** Focuses on the calculation of the "bounce" solution and Euclidean action in both flat and curved spacetime.
*   **Stochastic Framework:** Analyzes decay rates by solving the Fokker-Planck-Schrödinger eigenvalue problem in 1D and 2D.
*   **Synthesis:** Provides a direct comparison between stochastic results and the **Hawking-Moss** solution for decay in the presence of gravity.

---

## 🛠 Repository Structure

### Part 1: Semi-Classical Approach (Coleman)
Focuses on the instanton method and the calculation of the tunneling action $B$.

| Category | Features |
| :--- | :--- |
| **1D Solvers** | Custom Overshoot/Undershoot shooting algorithms and 1D `CosmoTransitions` implementations. |
| **2D Solvers** | 2D Path Deformation to find the most likely tunneling trajectory in coupled field spaces. |
| **Action Analysis** | Automated scans of action $B$ vs. potential parameters ($\gamma, \kappa_1, \kappa_2$). |

### Part 2: Stochastic Framework
Implements the Langevin/Fokker-Planck approach by solving the associated Schrödinger-like equation.

| Category | Features |
| :--- | :--- |
| **1D Dynamics** | Spectrum analysis of eigenvalues ($\Lambda_n/H$), eigenfunction visualization ($\psi_n$), and parameter sensitivity scans. |
| **2D Dynamics** | Coupled field stochastic evolution, 2D potential landscape mapping, and transition path visualization. |
| **Optimization** | Differential Evolution algorithms to fit potential parameters to target vacuum and barrier values. |
| **Comparison** | Direct cross-validation between Stochastic decay rates and Hawking-Moss solutions. |

---

## 💻 Technical Requirements

The numerical implementations use Python and the following scientific libraries:

- NumPy
- SciPy
- Matplotlib
- SymPy
- CosmoTransitions (for semiclassical bounce calculations)

Install the core dependencies:

```bash
pip install numpy scipy matplotlib sympy
```

For the specialized bounce solver, see the [CosmoTransitions GitHub repository](https://github.com/clwainwright/CosmoTransitions).

The scripts were developed for the thesis calculations and may require adjustments to paths, parameters, or package versions when executed in a different environment.
