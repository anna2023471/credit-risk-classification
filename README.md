# credit-risk-classification

Module 20 Report

## Overview of the Analysis

The purpose of this analysis was to predict which loans are at high resk of default.

The features used in the analysis were borrower income, number of accounts held, derogatory marks, loan size, interest rate, total debt, and the debt to income ratio.

The prediction was binary - whether the loan was healthy ('0') or at high risk of default ('1').

Logistic Regression, a supervised machine learning model, was used to make the predictions.

The data was split into two sets - a training set and a testing set. The training set was used to train the model to classify debt as healthy or high risk based on the features listed above. The testing set was used to evaluate how well the model could classify new data based on what it learnt from the training set.

## Results

The model's scores on classifying the testing dataset were as follows:

Accuracy: 99%

Precision:

    Healthy loans: 100%

    High risk loans: 87%

Recall:

    Healthy loans: 100%

    High risk loans: 89%

## Summary

The model's overall accuracy score is very high, owing to the large number of healthy loans in the dataset. The model's ability to correctly classify healthy loans is also high. However, its ability to correctlt classify high risk loans is significantly poorer.

A recall score of 89% for high risk loans (i.e. proportion of high risk loans that were correctly identified as such) means that the model will miss 11% of all those loans. Therefore, this model is not suitable for making lending decisions (deciding whether a loan should be approved) as incorrectly classifying 11% of high risk loans as healthy could results in significant financia losses; a model with a recall score of at least 95% is needed to make such decisions.

The model, however, is suitable for identifying customer who may be at risk of default for the pruposes of communication (e.g. reaching out to those customers to check on their financial situation or offer budgeting assistance to prevent loan default).


