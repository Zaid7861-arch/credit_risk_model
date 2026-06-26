Credit Risk Underwriting Predictor

Project Overview

This project simulates the core underwriting process used by financial institutions like American Express. By leveraging historical customer financial data (income, debt-to-income ratio, payment history, employment tenure), this machine learning model predicts the probability of an applicant defaulting on a credit product.

Problem Statement

Accurately distinguishing between creditworthy applicants and potential high-risk defaulters is critical to maintaining a healthy loan portfolio. This model employs Logistic Regression to provide a clear, interpretable risk assessment, allowing for data-driven credit approval decisions.

Technical Approach

Dataset Generation: Utilized sklearn.datasets.make_classification to create a synthetic dataset of 5,000 customers, featuring key financial indicators.

Data Preprocessing: Implemented StandardScaler to standardize financial variables. This ensures that features with larger numerical scales do not disproportionately influence the model coefficients, a critical step for linear models.

Modeling: Trained a Logistic Regression model, which is the industry standard for credit scoring due to its transparency and ability to output probability scores ($P(\text{Default})$).

Evaluation: Beyond standard accuracy, the model performance is assessed using the AUC-ROC (Area Under the Receiver Operating Characteristic Curve) score, which quantifies the model's ability to rank risk effectively across different classification thresholds.

Key Learnings

The Power of Scaling: Observed firsthand how standardizing data significantly improves the convergence and interpretability of Logistic Regression coefficients.

Metrics for Financial Stability: Recognized that in financial modeling, high accuracy does not always equal high performance; AUC-ROC and probability calibration are far more critical in determining the "separability" of risk profiles.

Business Impact: Understood how ML model outputs map directly to business risk appetite, helping lenders optimize the balance between approval rates and default protection.

Getting Started

Clone the repository.

Open Credit_Risk_LogisticRegression.ipynb in Google Colab or your local Jupyter environment.

Run the cells to see the model performance on the generated credit dataset.
