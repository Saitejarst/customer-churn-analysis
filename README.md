##Customer Churn Prediction – Data Science Project

##About the Project

This project is about predicting customer churn for a telecom company. Churn means customers who are leaving the service. The purpose of this project is to understand which type of customers are more likely to churn, and to build a machine learning model that can predict churn.

##Dataset

I used the Telco Customer Churn dataset which contains 7,043 rows and multiple columns like customer demographics, contract type, billing amount, tenure, and services. The target column is “Churn” which has Yes/No values.

##Steps I Completed

1. Data Understanding:-
I started by loading the dataset and checking the basic structure like number of rows, columns, data types, missing values, etc.
2. Data Cleaning:-
I found that the TotalCharges column was actually stored as string and had blank spaces, so I converted it to numeric and filled missing values. I also removed customerID because it does not help in prediction.
3. Exploratory Data Analysis (EDA):-
I plotted different graphs to see patterns between churn and features. I checked churn distribution, contract type vs churn, monthly charges vs churn, tenure vs churn, etc.
4. Feature Engineering:-
I encoded categorical variables using get_dummies, converted churn to 0 and 1, and split the data into training and testing sets.
5. Model Building:-
I trained two models: Logistic Regression and Random Forest.
6. Model Evaluation:-
I compared both models based on accuracy, recall and ROC-AUC.

##Observations from EDA

1. Customers with month-to-month contracts have higher churn.
2. Customers with higher monthly charges churn more.
3. Low tenure customers have higher churn.
4. Two year contract customers rarely churn.
5. Extra security services reduce churn risk

##Model Results

Logistic Regression:-
Accuracy: around 81%
Churn recall: around 57%
ROC-AUC: around 0.84

Random Forest:-
Accuracy: around 80%
Churn recall: around 50%
ROC-AUC: around 0.83

##Final Model Selection

Logistic Regression worked better because it had better recall for churn customers and a better ROC-AUC score. It is also easier to interpret compared to Random Forest.

##Business Suggestions

Based on the results, the company can reduce churn by:
1. Encouraging month-to-month customers to switch to long-term contracts
2. Giving discounts to high billing customers
3. Focusing on new customers with low tenure
4. Offering bundled services like tech support and security

##Tools Used

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook

##Project Structure

Project_CCP/
* 01_data_understanding.ipynb
* 02_data_cleaning.ipynb
* 03_eda.ipynb
* 04_feature_engineering.ipynb
* 05_model_building.ipynb
* Churn.csv

##Status

Project is completed end-to-end including EDA, model training, model evaluation and final insights.

##Author

Sai Teja,
Aspiring Data Scientist
