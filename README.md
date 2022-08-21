# Credit_Risk_Analysis

## Overview

This analysis uses machine learning to predict credit risk, testing the effectiveness of six different models. The first four models used logistic regression with four alternative sampling algorithms:

(1) Logistic regression w/RandomOverSampler  
(2) Logistic regression w/SMOTE  
(3) Logistic regression w/ClusterCentroids  
(4) Logistic regression w/SMOTEENN  

The last two models used ensemble classifiers:  

(5) Balanced Random Forest  
(6) Easy Ensemble Classifier  

These models are tested for their ability to predict credit risk, based on a dataset on consumer credit risk with 115,676 observations, containing over 100 variables on consumer's debts, assets, available credit, and credit histories. For each of these six models we calculate accuracy scores, generate confusion matrices, and imbalanced classification reports.

## Results

### Accuracy scores for the six models are:

(1) Accuracy Score for logistic regression w/RandomOverSampler: &ensp; 0.625  
(2) Accuracy Score for logistic regression w/SMOTE: &emsp; &emsp; &emsp; &emsp; &emsp; &nbsp; 0.651  
(3) Accuracy Score for logistic regression w/ClusterCentroids: &emsp; &ensp; &ensp; 0.516  
(4) Accuracy Score for logistic regression w/SMOTEENN: &emsp; &emsp; &emsp; &emsp; 0.650  
(5) Accuracy Score for Balanced Random Forest Classifier: &emsp; &emsp; &emsp; &nbsp; 0.788  
(6) Accuracy Score for Easy Ensemble Classifier: &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 0.920  

### Confusion matrices for the six models are:

(1) Logistic regression w/RandomOverSampler  
&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Predicted high_risk &emsp; &emsp; &ensp; Predicted low_risk  
Actual high_risk &emsp; &emsp; &emsp; 52 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 35  
Actual low_risk &emsp; &emsp; &emsp; 5952 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 11166  

(2) Logistic regression w/SMOTE  
&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Predicted high_risk &emsp; &emsp; &ensp; Predicted low_risk  
Actual high_risk &emsp; &emsp; &emsp; 56 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 31  
Actual low_risk &emsp; &emsp; &emsp; 5840 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 11278  

(3) Logistic regression w/ClusterCentroids  
&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Predicted high_risk &emsp; &emsp; &ensp; Predicted low_risk  
Actual high_risk &emsp; &emsp; &emsp; 52 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 35  
Actual low_risk &emsp; &emsp; &emsp; 9684 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 7434  

(4) Logistic regression w/SMOTEENN  
&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Predicted high_risk &emsp; &emsp; &ensp; Predicted low_risk  
Actual high_risk &emsp; &emsp; &emsp; 63 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 24  
Actual low_risk &emsp; &emsp; &emsp; 7256 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 9862  

(5) Balanced Random Forest  
&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Predicted high_risk &emsp; &emsp; &ensp; Predicted low_risk  
Actual high_risk &emsp; &emsp; &emsp; 58 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 29  
Actual low_risk &emsp; &emsp; &emsp; 1560 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 15558  

(6) Easy Ensemble Classifier  
&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Predicted high_risk &emsp; &emsp; &ensp; Predicted low_risk  
Actual high_risk &emsp; &emsp; &emsp; 78 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 9  
Actual low_risk &emsp; &emsp; &emsp; 975 &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 16143  

### Imbalanced Classification Reports for the six models are:

(1) Logistic regression w/RandomOverSampler  
&emsp; &emsp; &emsp; &emsp; &emsp; &ensp; pre &emsp; &emsp; &nbsp; rec &emsp; &emsp; spe &emsp; &emsp; &nbsp; f1 &emsp; &emsp; &nbsp; geo &emsp; &emsp; &nbsp; iba &emsp; &emsp; &nbsp; sup  
high_risk &emsp; &ensp; &nbsp; 0.01 &emsp; &emsp; 0.60 &emsp; &emsp; 0.65 &emsp; &emsp; 0.02 &emsp; &emsp; 0.62 &emsp; &emsp; 0.39 &emsp; &emsp; &ensp; 87  
low_risk &emsp; &emsp;  &nbsp; 1.00 &emsp; &emsp; 0.60 &emsp; &emsp; 0.60 &emsp; &emsp; 0.70 &emsp; &emsp; 0.62 &emsp; &emsp; 0.39 &emsp; &emsp; 17118  
avg/total &emsp; &emsp; 0.99 &emsp; &emsp; 0.65 &emsp; &emsp; 0.60 &emsp; &emsp; 0.78 &emsp; &emsp; 0.62 &emsp; &emsp; 0.39 &emsp; &emsp; 17205  

(2) Logistic regression w/SMOTE  
&emsp; &emsp; &emsp; &emsp; &emsp; &ensp; pre &emsp; &emsp; &nbsp; rec &emsp; &emsp; spe &emsp; &emsp; &nbsp; f1 &emsp; &emsp; &nbsp; geo &emsp; &emsp; &nbsp; iba &emsp; &emsp; &nbsp; sup  
high_risk &emsp; &ensp; &nbsp; 0.01 &emsp; &emsp; 0.64 &emsp; &emsp; 0.66 &emsp; &emsp; 0.02 &emsp; &emsp; 0.65 &emsp; &emsp; 0.42 &emsp; &emsp; &ensp; 87  
low_risk &emsp; &emsp;  &nbsp; 1.00 &emsp; &emsp; 0.66 &emsp; &emsp; 0.64 &emsp; &emsp; 0.79 &emsp; &emsp;  0.65 &emsp; &emsp; 0.42 &emsp; &emsp; 17118  
avg/total &emsp; &emsp; 0.99 &emsp; &emsp; 0.66 &emsp; &emsp; 0.64 &emsp; &emsp; 0.79 &emsp; &emsp; 0.65 &emsp; &emsp; 0.42 &emsp; &emsp; 17205  

(3) Logistic regression w/ClusterCentroids  
&emsp; &emsp; &emsp; &emsp; &emsp; &ensp; pre &emsp; &emsp; &nbsp; rec &emsp; &emsp; spe &emsp; &emsp; &nbsp; f1 &emsp; &emsp; &nbsp; geo &emsp; &emsp; &nbsp; iba &emsp; &emsp; &nbsp; sup  
high_risk &emsp; &ensp; &nbsp; 0.01 &emsp; &emsp; 0.60 &emsp; &emsp; 0.43 &emsp; &emsp; 0.01 &emsp; &emsp; 0.51 &emsp; &emsp; 0.26 &emsp; &emsp; &ensp; 87  
low_risk &emsp; &emsp;  &nbsp; 1.00 &emsp; &emsp; 0.43 &emsp; &emsp; 0.60 &emsp; &emsp; 0.60 &emsp; &emsp; 0.51 &emsp; &emsp; 0.26 &emsp; &emsp; 17118  
avg/total &emsp; &emsp; 0.99 &emsp; &emsp; 0.44 &emsp; &emsp; 0.60 &emsp; &emsp; 0.60 &emsp; &emsp; 0.51 &emsp; &emsp; 0.26 &emsp; &emsp; 17205  

(4) Logistic regression w/SMOTEENN  
&emsp; &emsp; &emsp; &emsp; &emsp; &ensp; pre &emsp; &emsp; &nbsp; rec &emsp; &emsp; spe &emsp; &emsp; &nbsp; f1 &emsp; &emsp; &nbsp; geo &emsp; &emsp; &nbsp; iba &emsp; &emsp; &nbsp; sup  
high_risk &emsp; &ensp; &nbsp; 0.01 &emsp; &emsp; 0.72 &emsp; &emsp; 0.58 &emsp; &emsp; 0.02 &emsp; &emsp; 0.65 &emsp; &emsp; 0.42 &emsp; &emsp;  &ensp; 87  
low_risk &emsp; &emsp;  &nbsp; 1.00 &emsp; &emsp; 0.58 &emsp; &emsp; 0.72 &emsp; &emsp; 0.73 &emsp; &emsp; 0.65 &emsp; &emsp; 0.41 &emsp; &emsp; 17118  
avg/total &emsp; &emsp; 0.99 &emsp; &emsp; 0.58 &emsp; &emsp; 0.72 &emsp; &emsp; 0.73 &emsp; &emsp; 0.65 &emsp; &emsp; 0.41 &emsp; &emsp; 17205  

(5) Balanced Random Forest  
&emsp; &emsp; &emsp; &emsp; &emsp; &ensp; pre &emsp; &emsp; &nbsp; rec &emsp; &emsp; spe &emsp; &emsp; &nbsp; f1 &emsp; &emsp; &nbsp; geo &emsp; &emsp; &nbsp; iba &emsp; &emsp; &nbsp; sup  
high_risk &emsp; &ensp; &nbsp; 0.04 &emsp; &emsp; 0.67 &emsp; &emsp; 0.91 &emsp; &emsp; 0.07 &emsp; &emsp; 0.78 &emsp; &emsp; 0.59 &emsp; &emsp; &ensp; 87  
low_risk &emsp; &emsp;  &nbsp; 1.00 &emsp; &emsp; 0.91 &emsp; &emsp; 0.67 &emsp; &emsp; 0.95 &emsp; &emsp; 0.78 &emsp; &emsp; 0.62 &emsp; &emsp; 17118  
avg/total &emsp; &emsp; 0.99 &emsp; &emsp; 0.91 &emsp; &emsp; 0.67 &emsp; &emsp; 0.95 &emsp; &emsp; 0.78 &emsp; &emsp; 0.62 &emsp; &emsp; 17205  

(6) Easy Ensemble Classifier  
&emsp; &emsp; &emsp; &emsp; &emsp; &ensp; pre &emsp; &emsp; &nbsp; rec &emsp; &emsp; spe &emsp; &emsp; &nbsp; f1 &emsp; &emsp; &nbsp; geo &emsp; &emsp; &nbsp; iba &emsp; &emsp; &nbsp; sup  
high_risk &emsp; &ensp; &nbsp; 0.07 &emsp; &emsp; 0.90 &emsp; &emsp; 0.94 &emsp; &emsp; 0.14 &emsp; &emsp; 0.92 &emsp; &emsp; 0.84 &emsp; &emsp; &ensp; 87  
low_risk &emsp; &emsp;  &nbsp; 1.00 &emsp; &emsp; 0.94 &emsp; &emsp; 0.90 &emsp; &emsp; 0.97 &emsp; &emsp; 0.92 &emsp; &emsp; 0.85 &emsp; &emsp; 17118  
avg/total &emsp; &emsp; 0.99 &emsp; &emsp; 0.94 &emsp; &emsp; 0.90 &emsp; &emsp; 0.97 &emsp; &emsp; 0.92 &emsp; &emsp; 0.85 &emsp; &emsp; 17205  

## Summary

The results of this analysis indicates that the Easy Ensemble Classifier model is superior to all other models and is recommended for use. This model:  

A) Has the highest accuracy score (0.920).  
B) Correctly identified the most high_risk loans (78 out of 87).  
C) Failed to identify the fewest high risk loans (9 out of 87 high risk loans identified as low risk).  
D) Flagged the fewest low risk loans as high risk (975 out of 17,118).  
E) Has the best recall (0.94) and F1 (0.97) scores.  
