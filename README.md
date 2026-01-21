# Fuzzy-NRS-TIS

This repository provides a reference implementation of the core methodology proposed in the IP&M manuscript:

> **Fuzzy Neighborhood Rough Set-Based Attribute Reduction over Temporal Information Systems with Application to Clinical Efficacy Evaluation**

The released code is intended to support **methodological transparency and reproducibility** of the proposed framework.

---

## Repository Structure

├── Phase-1/ # Unsupervised attribute reduction over temporal information systems
├── Phase-2/ # Temporal state estimation and three-way trend decision
├── README.md
├── LICENSE
└── .gitignore

---

## Method Overview

The implementation follows the two-stage framework described in the paper:

### Phase 1: Unsupervised Attribute Reduction
- Fuzzy neighborhood construction using Gaussian similarity
- Multi-β neighborhood modeling via quantile-based thresholds
- Rough-set-inspired lower/upper approximation analysis
- Greedy forward unsupervised attribute selection
- Attribute weight learning based on marginal contribution

### Phase 2: Temporal State Estimation and Trend Decision
- Linear Gaussian state-space modeling
- Parameter learning via EM algorithm
- RTS smoothing for latent state trajectories
- Standardized difference statistics (Δz / σΔ)
- Benjamini–Hochberg FDR for high-confidence decision thresholds
- EWMA-based temporal evidence accumulation
- Three-way decision outputs: **Improved / Worsened / Observe**

---

## Data Availability

Due to ethical approval constraints and data usage agreements with the data provider,  
the clinical follow-up data used in the study **cannot be shared publicly**, including any raw, processed, or derived versions.

Researchers interested in accessing the data should contact the data provider directly  
and follow the required application and approval procedures.

**This repository does not contain any clinical data.**

---

## Usage Notes

- The code is provided for research and reproducibility purposes.
- Users should prepare their own data according to the input format specified in the code.
- The released implementation focuses on the **core methodological pipeline**.
- Auxiliary scripts for ablation studies, sensitivity analysis, and experiment-specific visualization are not included, as they depend on restricted clinical data.

---

## License

This project is released under the MIT License.
