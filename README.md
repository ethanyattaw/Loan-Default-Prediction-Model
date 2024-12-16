# Loan-Default-Prediction-Model
XGBoost ML model predicting loan default status

## Overview

This project focuses on predicting loan defaults using a dataset containing various characteristics of loans and borrowers, such as demographic, financial, and loan-specific attributes. The model aims to identify patterns that indicate the likelihood of a loan defaulting, assisting financial institutions in making informed lending decisions. The project combines preprocessing, feature engineering, class balancing, hyperparameter tuning, and advanced modeling techniques. Two models are compared: Logistic Regression and XGBoost, with XGBoost achieving superior performance on all measures.

## Workflow and Features

1. **Dataset Exploration**:
   - Analyzed the data to identify missing values, outliers, and class imbalance (~78% non-default, ~22% default).

2. **Preprocessing**:
   - Handled missing values and capped outliers to ensure consistent data quality.
   - Encoded categorical variables and engineered new features like debt-to-income ratio and employment-to-age ratio.

3. **Class Balancing**:
   - Applied SMOTE (Synthetic Minority Oversampling Technique) to address the imbalance in the target variable.

4. **Modeling**:
   - Trained a baseline Logistic Regression model for comparison.
   - Trained and optimized an XGBoost model using grid search for hyperparameter tuning.

5. **Evaluation**:
   - Assessed both models on Accuracy, Precision, Recall, F1-Score, and ROC-AUC.
   - Presented confusion matrices for detailed error analysis.
  

## Results

| Metric                | Logistic Regression | XGBoost       |
|-----------------------|---------------------|---------------|
| **Accuracy**          | 0.855741            | 0.959372      |
| **Precision**         | 0.868170            | 0.988928      |
| **Recall**            | 0.838862            | 0.929146      |
| **F1-Score**          | 0.853264            | 0.958106      |
| **ROC-AUC**           | 0.923254            | 0.988098      |

- The XGBoost model achieved robust accuracy, outperforming Logistic Regression across all metrics.
