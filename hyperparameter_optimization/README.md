# Hyperparameter Optimization

A head-to-head comparison of three strategies for tuning a random forest on the digits dataset, all exploring the same search space with the same 5-fold cross-validation:

- **Grid search:** every one of the 720 combinations.
- **Random search:** 100 random combinations.
- **Bayesian optimization with Optuna (TPE):** 100 trials, each guided by the results of the previous ones.

The notebook explains how the Tree-structured Parzen Estimator decides where to sample next, and compares the strategies by best score, time, and how quickly each one converges. It also shows where Optuna's sampler concentrated its trials and which hyperparameters mattered most.

## Requirements

```
numpy
pandas
matplotlib
scikit-learn
optuna
```
