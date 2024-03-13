# Credit_Risk_Classification

Use various techniques to train and evaluate a model based on loan risk. I’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#Prerequisites)
- [Coding Instruction](#Coding-Instruction)
- [Analysis](#Analysis)
- [References](#references)
  
## Getting Started
Using various techniques train and evaluate a model based on loan risk.

## Prerequisites

Requirements for the software and other tools to build, test and push 

- [Jupyter Notebook](https://jupyter.org/)
- [scikit-learn](https://pypi.org/project/scikit-learn/)
- [Pathlib](https://pypi.org/project/pathlib/)  

## Coding Instruction

The instructions for this Challenge are divided into the following subsections:

  1. Split the Data into Training and Testing Sets
  2. Create a Logistic Regression Model with the Original Data
  3. Write a Credit Risk Analysis Report

#### Split the Data into Training and Testing Sets

Open the starter code notebook and use it to complete the following steps:

1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

- NOTE
  - A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

3. Split the data into training and testing datasets by using train_test_split.

#### Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:

1. Fit a logistic regression model by using the training data (X_train and y_train).

2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

3. Evaluate the model’s performance by doing the following:

    - Generate a confusion matrix.

    - Print the classification report.

4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

#### Write a Credit Risk Analysis Report

Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. 

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

1. An overview of the analysis: Explain the purpose of this analysis.

2. The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

3. A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

## Analysis

#### Overview of the Analysis

1. The analysis's goal is to develop and assess a loan risk-based model. Using a peer-to-peer lending services company's historical lending activity dataset, I developed a model that can determine a borrower's creditworthiness based on loan_status, the accuracy for healthy and high risk loans.

2. The following were the contents of the dataset: : loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and loan status.

3. The loan status, represented by variable y, is categorized as either 0 or 1,  where a loan is considered healthy if its value is 0 and it is considered high-risk of default if its value is 1. While everything else in the dataset falls under variable x.

4. The stages of the machine learning process I went through as part of this analysis:

  1. Data Collecting and Preparing
  2. Model Selection (Logistic Regression Model with the Original Data or Logistic Regression Model with Resampled Training Data)
  3. Model Training
  4.  Model Prediction
  5.  Model Utilization - Evaluate the model’s performance through:
        - Calculate the accuracy score of the model.
        - Generate a confusion matrix.
        - Printing the classification report.    
5. The accuracy score, confusion matrix, and classification report where all used as the basis for evaluating the model's performance.


#### Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

1. Machine Learning Model 1:

    - Logistic Regression: Accuracy: 0.9520479254722232 (95.2 %)

    - Precision: 0 ---> 1.00 , 1 ---> 0.85 

    - Recall Scores: 0 ---> 0.99 , 1 ---> 0.91

2. Machine Learning Model 2:

    - Logistic Regression: Accuracy: 0.9949885376126246 (99.4 %)

    - Precision: 0 ---> 1.00 , 1 ---> 0.99 
  
    - Recall Scores: 0 ---> 0.99 , 1 ---> 1.00 

## Summary

- My recommendation is to choose Model 2, Logistic Regression with Resampled Data, based on the comparison between  Model 1 and Model 2.This model performs well because it has better accuracy and recall scores.Given its greater recall score, the model is more adept at distinguishing between positive and negative samples. 

- The problem we are attempting to address will determine the performance, which will ultimately affect the outcomes the model produces.


## References

Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
