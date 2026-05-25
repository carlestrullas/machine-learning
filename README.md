# Machine Learning

---

## PAC1 — Environment Setup and Data Preparation

Flight price prediction dataset (India). Covers environment setup with Anaconda/Jupyter, dataset loading and merging, basic statistical and exploratory data analysis (outlier detection, correlation), categorical encoding and feature scaling, and dimensionality reduction with PCA and t-SNE.

## PAC2 — Unsupervised Learning and Image Analysis

Focuses on unsupervised learning techniques and their application to synthetic and image datasets. Covers classical clustering with k-means and the elbow rule, clustering of non-convex shapes with density-based and hierarchical methods, and feature engineering in polar coordinates to separate concentric structures. It also includes dimensionality reduction with PCA, t-SNE, and UMAP on the Iris and Digits datasets, reconstruction error analysis, clustering evaluation with ARI and confusion matrices, centroid visualization, image interpolation between cluster prototypes, and outlier detection with Isolation Forest.

## PAC3 — Supervised Learning and Regression Modeling

Explores supervised learning through both classification and regression tasks. It starts with visual classification experiments on EMNIST handwritten letters using KNN, SVM, and decision trees, including dimensionality reduction with UMAP, hyperparameter tuning, decision-boundary analysis, and model evaluation. It then applies a full regression workflow to a real used-car dataset, covering data cleaning, exploratory analysis, preprocessing, feature encoding, decision tree regression, metric-based assessment with $R^2$, RMSE, and MAE, and a comparative experiment with TabPFN for tabular prediction.

## PAC4 — Ensemble Learning and Cost-Sensitive Churn Prediction

Centers on advanced ensemble methods for a multiclass SaaS churn problem with class imbalance. Includes exploratory analysis and critical comparison between AI-generated hypotheses and dataset-specific evidence, robust preprocessing with stratified train/test split, and baseline model benchmarking. It implements and tunes Random Forest, Gradient Boosting, Stacking, Cascading (stacking with passthrough), and Balanced Random Forest using cross-validation and macro-F1 optimization, with detailed analysis of class-2 recall/precision trade-offs and feature importance. The PAC closes with post-training decision-threshold tuning on predicted probabilities to enforce high recall for critical churn cases and an economic impact analysis based on intervention and churn-loss costs.
