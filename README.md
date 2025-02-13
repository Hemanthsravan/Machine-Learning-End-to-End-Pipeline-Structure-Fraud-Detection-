# Machine-Learning-End-to-End-Pipeline-Structure-Fraud-Detection-
Automated Machine Learning Pipeline System
A robust, end-to-end Machine Learning pipeline designed to detect fraudulent transactions with high accuracy. This project implements an automated data processing and model training pipeline with dynamic resampling, advanced data handling, and optimized hyperparameter tuning.
Data Cleaning & Quality Checks:
Detects and handles missing values using Mode Imputation (categorical) & KNN Imputation (numerical).
Outlier capping with IQR, preventing data loss while keeping model performance high.
Skewness handling with Quantile Transformation to normalize highly skewed features dynamically.
Handling Class Imbalance:
Adaptive Resampling (ADASYN over SMOTE) based on class ratio analysis.
Resampling occurs inside Cross-Validation (CV) to prevent data leakage and improve generalization.
Model Training & Optimization:
GridSearchCV for hyperparameter tuning with resampling-aware cross-validation.
Supports multiple ML models (Logistic Regression, Random Forest, XGBoost, etc.).
Evaluates models using ROC-AUC, Precision-Recall Curve, F1-Score, and more.
