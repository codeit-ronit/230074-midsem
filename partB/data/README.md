# Dataset Documentation

This dataset was synthetically generated to test the Deterministic Anti-Annealing EM algorithm for Gaussian mixtures with heavily unbalanced mixing coefficients. 

## Structure
- `X.npy`: Contains exactly 2050 2D samples (features).
- `y.npy`: Contains the true cluster labels (0 or 1).

## Rationale
The paper notes that traditional EM struggles when highly unbalanced clusters (e.g. 2000 vs 50 points) overlap. This dataset enforces $\alpha_1 \approx 0.975$ and $\alpha_2 \approx 0.025$, with $\mu_1 = [0, 0]$ and $\mu_2 = [3, 0]$, creating a difficult overlapping condition that requires Anti-Annealing to resolve effectively in reasonable iterations.
