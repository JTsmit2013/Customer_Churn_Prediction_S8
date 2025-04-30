# 📉 Customer Churn Prediction (Beta Bank)

**Sprint 8 – Classification | Model Evaluation | Class Imbalance | Machine Learning**

Predicting customer churn is essential for Beta Bank, which faces gradual client loss month over month. This project builds a machine learning model to identify customers likely to leave the bank, helping the business take proactive steps for retention.

---

## 🔍 Project Overview

Retaining customers is significantly more cost-effective than acquiring new ones. Beta Bank aims to reduce churn by identifying which customers are at risk of leaving. This project focuses on:

- Developing a classification model with an **F1 score ≥ 0.59** on test data.
- Evaluating model robustness using **AUC-ROC** as a secondary metric.
- Addressing **class imbalance** to improve prediction reliability.

---

## 🎯 Objectives

- **Data Preparation**: Load, clean, and preprocess customer data.
- **Exploratory Data Analysis (EDA)**: Understand data distributions, class balance, and correlations.
- **Baseline Modeling**: Train initial models and evaluate without class balancing.
- **Model Optimization**: Handle class imbalance using upsampling and class weighting.
- **Evaluation & Testing**: Compare models and validate the best one on unseen data.

---

## 📁 Dataset Description

**File:** `/datasets/Churn.csv`

**Target Variable:**  
- `Exited`: 1 if the customer left the bank, 0 if they stayed.

**Features:**
- **Demographics**: `Geography`, `Gender`, `Age`, `Surname`
- **Financial Info**: `CreditScore`, `Balance`, `EstimatedSalary`, `NumOfProducts`, `HasCrCard`
- **Customer Behavior**: `Tenure`, `IsActiveMember`

---

## ⚙️ Methodology

- **Preprocessing**: Handled missing values, encoded categoricals, scaled numericals.
- **EDA**: Visualized feature distributions, explored churn rates, checked imbalance.
- **Model Selection**: Tested `DecisionTreeClassifier`, `RandomForestClassifier`, and `LogisticRegression`.
- **Class Imbalance Handling**: Applied **upsampling** and **class weighting**.
- **Hyperparameter Tuning**: Used `GridSearchCV` for optimization.
- **Final Evaluation**: Best model tested on a holdout dataset.

---

## 📊 Results Summary

- **Best Model:** `RandomForestClassifier` with **upsampled training data**
- **Test F1 Score:** `0.591`
- **AUC-ROC:** `0.838`
- ✅ The model **meets the required F1 threshold (≥ 0.59)**.
- 🔍 AUC-ROC confirms strong ability to distinguish between classes.

---

## 💡 Conclusion

- Three models were tested: Decision Tree, Random Forest, and Logistic Regression.
- **Random Forest** performed best and was optimized further.
- Among balancing strategies, **upsampling** yielded better results than class weighting.
- The final model provides **actionable insights** and can help Beta Bank **identify customers likely to churn**, with a good balance between precision and recall.

---

## 🛠️ Tools & Libraries

- Python 3.x
- pandas
- numpy
- scikit-learn
- seaborn & matplotlib (for EDA)
- Jupyter Notebook
