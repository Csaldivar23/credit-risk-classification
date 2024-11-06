# credit-risk-classification
Module_20_Challenge_Supervised_Learning

## Overview of the Analysis
For this assignment, I used various techniques to train and evaluate a model based on loan risk.
I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
The goal is to predict whether loans are healthy (denoted as 0) or high-risk (denoted as 1).

First, I imported the CSV data and converted it into a Pandas DataFrame. I then separated the data into labels `(y)` and features `(X)`.
After that, I split the data into training and testing datasets using `train_test_split`, with a random state of 1 to ensure reproducibility.

Next, I fitted the Logistic Regression model using the training data to learn the patterns in the dataset.
Once the model was trained, I made predictions on the testing data to evaluate its performance in identifying whether loans were healthy or high-risk.

To assess the model's performance, I generated a confusion matrix using the true labels from the testing set and the predictions made by the model.
I also printed a classification report that detailed the precision, recall, and F1-score for each class: healthy loans and high-risk loans.

## Results

* Logistic Regression Model:

    * Healthy Loans (0)
        * Precision Score: 1.00
        * Recall Score: 0.99
        * F1-Score: 1.00
        * Support: 18765

    * High-Risk Loans (1)
        * Precision Score: 0.84
        * Recall Score: 0.94
        * F1-Score: 0.89
        * Support: 619

## Summary

The Logistic Regression model worked well for predicting loan status.
It was excellent at identifying healthy loans, with a precision score of 1.00, meaning it correctly flagged all non-defaulting loans.
For high-risk loans, the model performed well with a precision of 0.84 and a recall of 0.94, though there's still some room for improvement.
Overall, this model is a solid choice for assessing loan risk in this dataset and can be applied effectively in similar use cases.