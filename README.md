# Customer-Churn-
Predicting whether the customer will churn or not churn based on the previous history

# Problem Statement

In the highly competitive telecommunications industry, retaining customers is a major challenge. Customer churn—when customers stop using a company's services—can result in significant revenue loss. Identifying potential churners in advance enables companies to take proactive retention measures.

Problem: Predict whether a customer will churn based on historical data about customer demographics, account information, and services used.

# Objective

To build and evaluate multiple classification models to predict customer churn and determine the most effective model for accurate predictions. Ultimately, the goal is to use these insights to improve customer retention strategies.

# Dataset Description

* Dataset: Telco Customer Churn

* Source: IBM Sample Data (commonly used for churn prediction)

* Number of Records: 7,043 customers

* Number of Features: 21 columns (20 features + 1 target)

# Feature Description

* customerID -------> Unique ID for each customer

* gender------------> Male/Female

* SeniorCitizen--------> Whether the customer is a senior citizen (0 or 1)

* Partner, Dependents -----> Marital and dependent status

* tenure ------> Number of months the customer has stayed

* PhoneService, MultipleLines ------> Phone service usage

* InternetService, OnlineSecurity, OnlineBackup----> Internet service types and add-ons

* Contract, PaperlessBilling, PaymentMethod---------> Billing and contract information

* MonthlyCharges, TotalCharges----------> Charges for the customer

* Churn -----------> Target variable (Yes/No)

# Approach

1. Data Preprocessing

* Handled missing or inconsistent values (especially in TotalCharges)

* Converted categorical variables to numeric using one-hot encoding

* Scaled numerical features where needed

2. Train-Test Split

* Split the data into training and testing sets (typically 70/30 or 80/20 split)

3. Model Selection and Evaluation

The following classification algorithms were implemented and evaluated:

 Models                                          Accuracy(%)
 
Logistic Regression       ------------->        78.53 

Decision Tree Classifier ------------->         77.82

Random Forest Classifier  ------------->        80.52

Gradient Boosting Classifier ------------->     77.67

XGBoost Classifier         ------------->       79.53 

Support Vector Machine (SVM) ------------->     79.53

# Conclusion

The Random Forest Classifier outperformed all other models in predicting customer churn with the highest accuracy and balanced performance across all evaluation metrics. It provides robustness to overfitting, handles both categorical and numerical features well, and offers feature importance for business interpretability.

 




