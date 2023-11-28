# Overview

In this Module we will use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

We will perform below three activities 

1.Split the Data into Training and Testing Sets

2.Create a Logistic Regression Model with the Original Data

3.Write a Credit Risk Analysis Report

To perform this analysis, we use Machine Learning techniques to train and evaluate the data.
We resample the dataset using  RandomOverSampler module from the imbalanced-learn library.
We then Predict a Logistic Regression Model with Resampled Training Data and evaluate the results and provide a comparison for our analysis. 

# The Results
Logistic Regression Model 1:
	• Precision:  the model was 100% precise in predicting low-risk loans,, though the model was only 87% precise in predicting high-risk loans
	• Accuracy: 94%
	• Recall: the model had 100% recall in predicting low-risk loans, but 89% recall in predicting high-risk loans
	
Logistic Regression Model 2:
	• Precision: the model was the model was 100% precise in predicting low-risk loans, , though the model was only 87% precise in predicting high-risk loans
	• Accuracy: 100%
	• Recall: 100%

# Summary
Logistic Regression Model 2 is less likely to predict false negative results. However, based on the confusion matrices for each model, Logistic Regression Model 2 predicted slightly more false positives (low-risk when the actual was high-risk).

If the goal of the model is to determine the likelihood of high-risk loans, neither model scores above 90% precision. Logistic Regression Model 2 had fewer false predictions of the testing data overall and would be the best model to use based on the high accuracy and recall of this model.


