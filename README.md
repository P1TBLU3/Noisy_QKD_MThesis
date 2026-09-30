# Information Leakage and Quantum Cloning in BB84

This repository contains the computational work developed during my Master's Thesis on **information leakage, disturbance, and eavesdropping strategies in BB84 quantum key distribution**.

It includes both the final analysis presented in the thesis and earlier exploratory studies that were part of the research process.

## Repository Structure

```text
.
├── 01_information_leakage.ipynb
├── 02_povm_gentle_measurements_approach.ipynb
├── 03_leakage_cloning_region.ipynb
├── requirements.txt
├── README.md
└── MT_NoisyQKD.pdf
```


## Notebooks

### 01 — Information Leakage Fundamentals

`01_information_leakage.ipynb`

Introduces the information-leakage framework used throughout the project.

It includes:

- A simplified BB84 intercept-resend model.
- QBER and Shannon mutual-information calculations.
- Implementation of the leakage/gentleness optimization.
- Reproduction of a reference leakage-versus-gentleness result.

This notebook represents an **early validation and exploratory stage** of the research and is not directly included in the final thesis results.

### 02 — Custom POVM Approach

`02_povm_gentle_measurements_approach.ipynb`

Explores several manually defined POVM-based eavesdropping strategies and studies the trade-off between **information leakage and disturbance**.

It includes:

- Weak gentleness and disturbance calculations.
- Several custom POVM constructions.
- Leakage evaluation under different measurement parameters.
- Analysis in the presence of channel noise.
- Comparison between different candidate measurement strategies.

This notebook is also **exploratory work** that helped motivate the more systematic approach used in the final study.

### 03 — Leakage and Cloning Region

`03_leakage_cloning_region.ipynb`

Contains the main computational study associated with the Master's Thesis.

It includes:

- Construction of the asymmetric quantum cloning region.
- Mapping cloning parameters to leakage and disturbance.
- Analysis under depolarizing channel noise.
- Comparison between Eve's information leakage and the Alice-Bob channel capacity.
- Study of the standard 11% BB84 QBER reference point.
- Evaluation of the model-specific information-balance condition

$$\Delta_{\text{info}} = C_{AB} - L_E$$

This notebook contains the analysis most closely related to the results presented in the thesis.

## Thesis

The complete Master's Thesis is included as a PDF in the repository:

```text
Master_Thesis.pdf
```

The thesis provides the theoretical background, mathematical formulation, methodology, interpretation of the results, and complete discussion of the final study.

## Installation

Install the Python dependencies with:

```bash
pip install -r requirements.txt
```

The notebooks can then be executed with Jupyter Notebook, JupyterLab, or a compatible IDE such as Visual Studio Code.

## Research Progression

The notebooks are ordered according to the development of the research:

```text
Information Leakage Fundamentals
            ↓
Exploratory Custom POVMs
            ↓
Asymmetric Quantum Cloning Region
            ↓
Final Thesis Analysis
```

The first two notebooks are kept in the repository to document the exploratory work that led to the methodology used in the final thesis.
