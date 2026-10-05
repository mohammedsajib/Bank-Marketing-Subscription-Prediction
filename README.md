# Bank Marketing Subscription Prediction

A real-world machine learning classification project that predicts whether a bank customer will subscribe to a term deposit after a marketing campaign.

## Project Overview

The goal of this project is to help banks identify customers who are more likely to subscribe to a term deposit based on demographic, financial, and campaign-related information.

**Dataset:** UCI Bank Marketing Dataset
**Rows:** 45,211
**Features:** 16
**Task:** Binary Classification

## Machine Learning Pipeline

```text
Data Loading
     ↓
Data Preprocessing
     ↓
Train/Test Split
     ↓
One-Hot Encoding + Scaling
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Model Comparison
```

## Models

Three machine learning algorithms were evaluated:

* Logistic Regression
* Random Forest
* XGBoost

## Results

| Model               |   Accuracy | Yes Recall |   Yes F1 |
| ------------------- | ---------: | ---------: | -------: |
| Logistic Regression |     90.12% |        35% |     0.45 |
| Random Forest       |     90.61% |        40% |     0.50 |
| **XGBoost**         | **91.06%** |    **49%** | **0.56** |

XGBoost was selected as the final model based on its overall performance and improved ability to identify positive (`yes`) customers.

The target variable is imbalanced: **88.30% no** and **11.70% yes**. Therefore, precision, recall, and F1-score were considered alongside accuracy.

## Technologies

Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, and Joblib.

## Future Improvements

* Hyperparameter tuning
* SHAP explainability
* Threshold optimization
* FastAPI deployment
* Docker containerization

## Author

**Mohammed Sajib**
Aspiring AI/ML Engineer
