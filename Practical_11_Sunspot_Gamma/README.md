# Practical 11: Bayesian & Frequentist Gamma Modeling of Sunspot Counts

## Overview
This practical models historical monthly sunspot counts (`Datasets/sunspots.csv`, January 1749 – November 2018) using a shifted Gamma distribution ($Y + 1 \sim \text{Gamma}(a, b)$) and compares Maximum Likelihood Estimation (MLE) against Bayesian Markov Chain Monte Carlo (MCMC) inference.

## Methodology
1. **Time-Series Exploration:** Visualizes ~11-year solar cycles and quantifies sample skewness.
2. **12-Year Epoch Folding:** Partitions the series into 144-month blocks and fits a scaled Gamma curve to the composite cycle profile.
3. **Maximum Likelihood Benchmark:** Computes MLE estimates $(\hat{a}_{\text{MLE}}, \hat{b}_{\text{MLE}})$ on shifted observations ($y + 1$).
4. **Log-Space Metropolis-Hastings MCMC:** Proposes random-walk steps in unconstrained $(\log a, \log b)$ space with the exact Jacobian adjustment ($+\log a + \log b$) across three regimes (first 50 months, full catalog, last 50 months).
5. **Diagnostics & Posterior Predictive Checks:** Evaluates chain mixing, trace stability, 95% credible intervals, and simulated predictive distributions.

## How to Run
Ensure `sunspots.csv` is placed in `../Datasets/sunspots.csv`, then run:
```bash
jupyter notebook Practical_11_Sunspot_Gamma.ipynb
```
