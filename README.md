# Customer Churn Prediction using Machine Learning

This project applies supervised machine learning models to predict customer churn based on telecom user behavior and demographics. It includes data cleaning, preprocessing, feature engineering, model training (Logistic Regression & Random Forest), and performance evaluation.

---

## Project Overview

- Binary classification problem (Churn or Not)
- Goal: Identify customers likely to churn for proactive retention strategies
- Dataset includes service usage, contract types, billing methods, and demographics

---

## Algorithms Used

-  Logistic Regression (with feature scaling)
-  Random Forest Classifier (with default settings)

---

## Data Summary

**Features**:
- Categorical: `gender`, `SeniorCitizen`, `Partner`, `InternetService`, etc.
- Numerical: `tenure`, `MonthlyCharges`, `TotalCharges`
- Target: `Churn` (Yes/No → 1/0)

**Preprocessing**:
- Converted `TotalCharges` to numeric
- Handled missing values
- Mapped binary fields
- One-hot encoding for categorical variables

---

## Model Development Steps

1. **Preprocessing**
   - Dropped `customerID`, converted booleans
   - Handled missing `TotalCharges` values
   - Applied one-hot encoding

2. **Train-Test Split**
   - 80/20 split with `random_state=42`

3. **Feature Scaling**
   - StandardScaler applied to Logistic Regression

4. **Model Training**
   - Trained `LogisticRegression` and `RandomForestClassifier` from scikit-learn

---

##  Model Evaluation

### Logistic Regression  
- Accuracy: **0.79**  
- Precision (Churn): **0.62**  
- Recall (Churn): **0.52**  
- F1-Score (Churn): **0.56**

###  Random Forest  
- Accuracy: **0.79**  
- Precision (Churn): **0.63**  
- Recall (Churn): **0.48**  
- F1-Score (Churn): **0.54**

###  Confusion Matrix (Random Forest)
- Visualized with Seaborn for better interpretability

---

## Outputs

- `logistic_regression_model_scaled.pkl`
- `random_forest_model.pkl`
- `processed_customer_data.csv`

---

## Author

**Abhi Sharma**  
Machine Learning Project – Internshala Training

---

## Status

✔️ Completed  
 Includes: Cleaned dataset, trained models, visualizations

---

 This project demonstrates practical machine learning skills in binary classification, model evaluation, and feature engineering for customer churn analysis.
