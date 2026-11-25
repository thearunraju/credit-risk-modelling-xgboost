# Credit Risk Modelling using XGBoost

## Project Overview
This project develops a machine learning model to predict whether a credit card customer is likely to default on their next month's payment.

The objective is to analyse customer credit behaviour, build predictive models, evaluate their performance, and identify the key factors influencing default risk.

## Dataset
- **Source:** UCI Machine Learning Repository
- **Dataset:** Default of Credit Card Clients
- **Records:** 30,000 customers
- **Features:** 23 input features
- **Target:** Next-month payment default (0 = No Default, 1 = Default)

## Models Used
1. Logistic Regression (Baseline Model)
2. XGBoost Classifier

## Methodology
- Data loading and exploration
- Exploratory Data Analysis (EDA)
- Train-test split with stratification
- Model training and evaluation
- Confusion matrix analysis
- ROC curve analysis
- Model interpretation using SHAP

## Model Performance

| Metric | Logistic Regression | XGBoost |
|---|---:|---:|
| Accuracy | 67.97% | 76.70% |
| Precision | 36.72% | 47.94% |
| Recall | 62.02% | 62.17% |
| F1-Score | 46.13% | 54.13% |
| ROC-AUC | 70.81% | 77.75% |

XGBoost outperformed the Logistic Regression baseline across all reported evaluation metrics.

## Model Explainability

SHAP (SHapley Additive exPlanations) was used to interpret model predictions and identify the most influential features.

The top contributing features included:
- Recent repayment status
- Credit limit
- Recent bill amount
- Previous payment amounts

Recent repayment behaviour emerged as the strongest predictor of credit default.

## Key Takeaways
- XGBoost achieved better predictive performance than the Logistic Regression baseline.
- Class imbalance was addressed using class weighting.
- SHAP provided insights into the factors influencing model predictions.
- Recent repayment behaviour played the most significant role in predicting credit default.

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, SHAP, Jupyter Notebook.
