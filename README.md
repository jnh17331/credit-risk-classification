# Loan Activity Analysis

## Table of Contents
- [Introduction](#introduction)
- [Importing the Data](#importing-the-data)
- [Logistic Regression Model](#logistic-regression-model)
- [Resampled Model](#resampled-model)

## Introduction
In this exercise, we explore a machine learning model designed to make decisions on identifying the creditworthiness of borrowers.

## Importing the Data

First, I imported the csv file including the data shown below

|   loan_size   | interest_rate | borrower_income | debt_to_income | num_of_accounts | derogatory_marks | total_debt |
|--------------:|--------------:|----------------:|---------------:|----------------:|-----------------:|-----------:|
|       10700.0 |         7.672 |           52800 |       0.431818 |               5 |                1 |      22800 |
|        8400.0 |         6.692 |           43600 |       0.311927 |               3 |                0 |      13600 |
|        9000.0 |         6.963 |           46100 |       0.349241 |               3 |                0 |      16100 |
|       10700.0 |         7.664 |           52700 |       0.430740 |               5 |                1 |      22700 |
|       10800.0 |         7.698 |           53000 |       0.433962 |               5 |                1 |      23000 |


Next, we fit our model to our data using the split data from the table using the sklearn library.

## Logistic Regression Model
- Fit our Logistic Regression Model to our Data Model
- Predict the testing data
- Go over results of the model (Classification Report Below)

```python
---------------Classification Report-----------------
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384
-----------------------------------------------------
```

## Resampled Model

We also did another model with the same data, just resampled to test the model under different conditions. Note that it did have a slightly higher accuracy in the recall in this model, but there is no noticeable difference.
