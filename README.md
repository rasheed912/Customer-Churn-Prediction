# Customer Churn Prediction Project

## Project Objective

The objective of this project is to predict whether a bank customer is likely to leave the bank (customer churn) using machine learning techniques.

Customer churn is a major challenge for banks because losing customers can reduce revenue and increase customer acquisition costs. This project helps identify customers who are at high risk of leaving the bank using customer demographics, account activity, and financial information.

This is a **binary classification problem**, where the target variable is:

* `Exited`

  * 1 → Customer Left the Bank (Churn)
  * 0 → Customer Stayed with the Bank

---

# Dataset Description

The project uses the:

### Churn Modelling Dataset

The dataset contains customer banking information and account-related details.

## Features Used

### Customer Information

* CreditScore
* Geography
* Gender
* Age
* Tenure

### Banking Information

* Balance
* NumOfProducts
* HasCrCard
* IsActiveMember

### Financial Information

* EstimatedSalary

### Target Variable

* Exited (Target)

---

# Project Workflow

## 1. Data Understanding

* Loaded dataset using Pandas
* Explored dataset structure and feature information
* Checked dataset dimensions and data types
* Identified target variable (`Exited`)

---

## 2. Data Cleaning and Preparation

Performed preprocessing steps:

* Removed unnecessary columns:

  * RowNumber
  * CustomerId
  * Surname

* Checked missing values

* Encoded categorical variables:

  * Label Encoding for Gender
  * One-Hot Encoding for Geography

* Prepared dataset for machine learning model training

---

## 3. Exploratory Data Analysis (EDA)

Visual analysis was performed to understand customer churn patterns.

### Visualizations Included

* Customer churn distribution
* Gender vs churn
* Age distribution
* Balance distribution
* Correlation heatmap
* Feature importance graph

### Key Insights from EDA

* Older customers are more likely to churn
* Inactive customers show higher churn rates
* Customers with fewer products tend to leave more
* Geography influences churn behavior
* High account balance customers may churn more frequently

---

## 4. Model Building

Machine learning classification model used:

* Random Forest Classifier

### Steps

* Defined feature set (X) and target variable (y)
* Split dataset into training and testing sets
* Trained Random Forest model on training data
* Predicted customer churn on test data

---

## 5. Model Evaluation

The model was evaluated using:

### Metrics

* Accuracy Score
* Confusion Matrix
* Classification Report
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

### Confusion Matrix

Used to measure:

* True Positives
* True Negatives
* False Positives
* False Negatives

---

# Results and Insights

## Key Insights

* Age is one of the most important churn indicators
* Active members are less likely to leave the bank
* Number of products strongly affects customer retention
* Customer geography impacts churn behavior
* Balance and credit score influence churn probability

---

## Model Performance

* Random Forest Classifier achieved good prediction accuracy
* Model successfully identified churn customers
* Feature importance analysis improved business understanding
* Confusion matrix showed effective classification performance

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Conclusion

This project successfully builds a machine learning system for customer churn prediction using banking customer data.

It includes:

* Data preprocessing and cleaning
* Exploratory Data Analysis (EDA)
* Feature encoding
* Classification model training
* Model evaluation and feature importance analysis

### Final Outcome

The system can help banks:

* Identify customers likely to leave
* Improve customer retention strategies
* Reduce customer churn
* Support data-driven business decisions

---

# Future Improvements

* Use advanced models such as XGBoost and LightGBM
* Perform hyperparameter tuning
* Handle class imbalance using SMOTE
* Deploy model using Flask or Streamlit
* Improve evaluation using ROC-AUC score and cross-validation

