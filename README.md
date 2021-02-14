# Issuing-Credit-Cards-and-SQL-Assignment
Metis Project 3 w/ Starters

By: Gabriel Equitz
______________________________________________________

## Problem Statement
- A credit card startup needs a supervised learning model to avoid defaults
- Both user and company desire to avoid credit card debt and failure to pay
- The model will collect data from credit card applicants (e.g age) which will help us make a predictive model
- The target of the model is to calculate the probability that a borrower is going to default next month

## Data Sources
- The project contains 1 csv file: UCI_Credit_Card.csv. It contains 30,000 rows and 25 columns, containing data of variables such as Gender, Education, Marriage Status, and Pay Over Balance.
- https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset
- https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients

## Methodology
- Get the UCI data and perform data cleaning
- EDA and finding best features for our model
- Continued Data cleaning
- Accuracy is the chosen metric, which we will check against different methods: XGBoost, Logistic Regression, Naive Bayes, Random Forest, and KNN
- Divide the data into training and testing, which consisted of 25% of the total
- Measure the performance of the model on the testing data, using our metrics

## Findings
- We determine our 5 independent variables to be Pay_0 (measure how delayed the borrower is in their payment), log_limit_bal (logarithm of limit balance), aver_pay_over_balance (average of 6 months of payment amount over the outstanding balance), sex (dummy variable, with Male = 1, Female = 0), married (dummy variable, with Married = 1, Single = 0)
- log_limit_bal had greatest coeff = -0.949
- Married and women were less likely to default
- Accuracy (0.818) and AuC (0.754) were highest with XGBoost

## Libraries and Notebook used
- [Jupyter](https://jupyter.org/)
- [Matplotlib](https://matplotlib.org/)
- [Numpy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Seaborn](https://seaborn.pydata.org/)
- [XGBoost](https://xgboost.readthedocs.io/en/latest/)

## Blog links
- TBD
