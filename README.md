# Customer_Churn_Prediction_S8

# **Customer Churn Prediction for Beta Bank**

## **Project Overview**  
Beta Bank is experiencing customer churn, with clients gradually leaving each month. Retaining existing customers is more cost-effective than acquiring new ones, making it essential to predict potential churn early.  

This project focuses on developing a machine learning model to predict whether a customer will leave the bank soon, using historical customer data. The objective is to maximize the **F1 score**, with a minimum threshold of **0.59** on the test set. The **AUC-ROC** metric is also analyzed for additional evaluation.  

## **Objectives**  
- **Data Preparation:** Load, clean, and preprocess customer data.  
- **Exploratory Data Analysis (EDA):** Understand data distributions, feature importance, and class balance.  
- **Baseline Modeling:** Train an initial model without addressing class imbalance and analyze results.  
- **Model Optimization:** Implement at least two techniques to handle class imbalance and fine-tune hyperparameters.  
- **Evaluation & Testing:** Compare models based on F1 score and AUC-ROC, selecting the best-performing one.  

## **Dataset Description**  
The dataset is stored in **`/datasets/Churn.csv`** and contains the following features:  

### **Features**  
- **Demographics:** `Geography`, `Gender`, `Age`, `Surname`  
- **Financial Information:** `CreditScore`, `Balance`, `EstimatedSalary`, `NumOfProducts`, `HasCrCard`  
- **Customer Behavior:** `Tenure`, `IsActiveMember`  

### **Target Variable**  
- `Exited`: **1** if the customer left the bank, **0** if they stayed.  

## **Methodology**  
1. **Data Preprocessing:** Handle missing values, encode categorical variables, and scale numerical features.  
2. **Exploratory Data Analysis:** Examine feature distributions, correlations, and class imbalance.  
3. **Baseline Model:** Train an initial classifier without addressing class imbalance.  
4. **Class Imbalance Handling:** Apply **oversampling, undersampling, or class weighting** to improve predictions.  
5. **Model Training & Selection:** Train multiple models, validate their performance, and tune hyperparameters.  
6. **Final Evaluation:** Assess the best model on unseen data, ensuring an **F1 score ≥ 0.59**, while analyzing AUC-ROC.  

## **Performance Metrics**  
- **F1 Score:** Primary metric to balance precision and recall.  
- **AUC-ROC:** Measures model performance across different classification thresholds.  

## **Conclusion**  
This project provides a data-driven approach to customer retention, helping Beta Bank proactively identify and retain customers at risk of leaving.  
