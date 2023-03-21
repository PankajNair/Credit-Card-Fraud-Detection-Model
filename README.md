# Credit Card Fraud Detection Model
## Problem Statement
Credit card fraud is a major concern for financial institutions and cardholders. Fraudsters use various techniques to steal credit card information and make unauthorized transactions, which can result in significant financial losses for both the card issuer and the cardholder. Traditional fraud detection methods often fail to detect new and sophisticated fraud patterns, leading to increased losses. Therefore, developing an accurate and reliable machine learning model for credit card fraud detection has become an urgent need.
## Data Information
The dataset can be download using this [link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

The dataset contains transactions made by credit cards in September 2013 by European cardholders.

This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions. It contains only numerical input variables which are the result of a PCA transformation. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.
## Project Pipeline
* Understanding the Data:  We load the data into a dataframe using Pandas and understand the features present in it. This helps in choosing the features that will be needed for the final model.
* Data Preprocessing: Data preprocessing is the essential step of cleaning and transforming raw data to make it suitable for machine learning models. As the current dataset is highly unbalanced, we undersample the data to make it balanced for more accurate predictions.
* Train/Test Split: The data is split into two sets: one for training the model and the other for testing its performance. We use the train_test_split function available in the sklearn library to perform the operation.
* Model Training and Evaluation: Here we can try different models until we get the desired level of performance on the given dataset. We use the Decision Tree Classifier as our model availabe in the sklearn library. We also need to evaluate the models using appropriate evaluation metrics.
