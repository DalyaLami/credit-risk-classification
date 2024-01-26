# Module 12 Report Template

## Overview of the Analysis

* The analysis's goal is to develop and assess a loan risk-based model. Using a peer-to-peer lending services company's historical lending activity dataset, I developed a model that can determine a borrower's creditworthiness based on loan_status, the accuracy for healthy and high risk loans.

* The following were the contents of the dataset: : loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and loan status.

* The loan status, represented by variable y, is categorized as either 0 or 1,  where a loan is considered healthy if its value is 0 and it is considered high-risk of default if its value is 1. While everything else in the dataset falls under variable x.

* The stages of the machine learning process I went through as part of this analysis:

        1- Data Collecting and Preparing

        2- Model Selection (Logistic Regression Model with the Original Data or Logistic Regression Model with Resampled Training Data)

        3- Model Training

        4- Model Prediction

        5- Model Utilization (Evaluate the model’s performance through:              - Calculate the accuracy score of the model.
                    - Generate a confusion matrix.
                    - Printing the classification report.)
                    
* The accuracy score, confusion matrix, and classification report where all used as the basis for evaluating the model's performance.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

  * Logistic Regression: Accuracy: 0.9520479254722232 (95.2 %)

  * Precision: 0 ---> 1.00 , 1 ---> 0.85 

  * Recall Scores: 0 ---> 0.99 , 1 ---> 0.91

* Machine Learning Model 2:

  * Logistic Regression: Accuracy: 0.9949885376126246 (99.4 %)

  * Precision: 0 ---> 1.00 , 1 ---> 0.99 

  * Recall Scores: 0 ---> 0.99 , 1 ---> 1.00 

## Summary

* My recommendation is to choose Model 2, Logistic Regression with Resampled Data, based on the comparison between  Model 1 and Model 2.This model performs well because it has better accuracy and recall scores.Given its greater recall score, the model is more adept at distinguishing between positive and negative samples. 

* The problem we are attempting to address will determine the performance, which will ultimately affect the outcomes the model produces.
