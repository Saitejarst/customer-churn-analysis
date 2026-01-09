##Customer Churn Prediction – Data Science Project

##About the Project
This project is about predicting customer churn for a telecom company. Churn means customers who are leaving the service. The purpose of this project is to understand which type of customers are more likely to churn, and to build a machine learning model that can predict churn.

##Dataset
I used the Telco Customer Churn dataset which contains 7,043 rows and multiple columns like customer demographics, contract type, billing amount, tenure, and services. The target column is “Churn” which has Yes/No values.

##Steps I Completed

1. Data Understanding
I started by loading the dataset and checking the basic structure like number of rows, columns, data types, missing values, etc.
2. Data Cleaning
I found that the TotalCharges column was actually stored as string and had blank spaces, so I converted it to numeric and filled missing values. I also removed customerID because it does not help in prediction.
3. Exploratory Data Analysis (EDA)
I plotted different graphs to see patterns between churn and features. I checked churn distribution, contract type vs churn, monthly charges vs churn, tenure vs churn, etc.
4. Feature Engineering
I encoded categorical variables using get_dummies, converted churn to 0 and 1, and split the data into training and testing sets.
5. Model Building
I trained two models: Logistic Regression and Random Forest.
6. Model Evaluation
I compared both models based on accuracy, recall and ROC-AUC.

##Observations from EDA

* Customers with month-to-month contracts have higher churn.
* Customers with higher monthly charges churn more.
* Low tenure customers have higher churn.
* Two year contract customers rarely churn.
* Extra security services reduce churn risk.

* 
