# Practical 12: Metropolis-Hastings Algorithm & Deterministic Solar Cycle Modeling

## Overview
This practical contrasts stochastic Bayesian sampling against deterministic mathematical modeling across two parts:
- **Part A (Stochastic MCMC):** Implements a numerically stable log-posterior Metropolis-Hastings sampler for a Binomial-Beta conjugate coin-flip model ($k = 21$ heads out of $n = 30$ flips) and benchmarks sampled draws against the exact $\text{Beta}(22, 10)$ distribution.
- **Part B (Deterministic Modeling):** Fits a four-parameter squared-sinusoid harmonic equation $\text{count}(t) = c_0 + A \sin^2(\pi (t - t_0)/P)$ to historical sunspot data (`Datasets/sunspots.csv`), analyzes residual distributions, and verifies deterministic forecast reproducibility.

## Key Highlights
- **Log-Posterior Evaluation:** Prevents floating-point underflow in Metropolis acceptance ratios.
- **Proposal Step-Width Tuning:** Evaluates mixing behavior and acceptance rates across $\sigma \in \{0.01, 0.12, 0.45, 2.50\}$.
- **2D Grid-Initialized Curve Fitting:** Finds globally consistent solar cycle period ($P$) and phase ($t_0$) parameters via non-linear least squares.

## How to Run
Ensure `sunspots.csv` is placed in `../Datasets/sunspots.csv`, then run:
```bash
jupyter notebook Practical_12_Metropolis_and_Deterministic.ipynb
```
