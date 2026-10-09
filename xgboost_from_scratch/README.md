# XGBoost from Scratch

A from-first-principles implementation of XGBoost in NumPy, benchmarked against the official `xgboost` library.

The notebook derives the regularised second-order objective, the closed-form optimal leaf weight and the split gain formula, and maps each of them directly onto code:

- `Node` and `Tree`: exact greedy split search with vectorised gain computation.
- `BaseCustomXGBoost`: the shared boosting loop, with pluggable gradient and hessian.
- `CustomXGBoostRegressor` (squared error) and `CustomXGBoostClassifier` (log loss).

Both models are evaluated on synthetic regression and binary classification tasks, with learning curves and side-by-side comparisons against the native implementation.

## Requirements

```
numpy
pandas
matplotlib
scikit-learn
xgboost
```
