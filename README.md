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

(1) Accuracy Score for logistic regression w/RandomOverSampler:       0.6249984891886339
(2) Accuracy Score for logistic regression w/SMOTE:                   0.6512584051472337
(3) Accuracy Score for logistic regression w/ClusterCentroids:        0.5159904274991842
(4) Accuracy Score for logistic regression w/SMOTEENN:                0.6501283182453639
(5) Accuracy Score for Balanced Random Forest Classifier:             0.7877672625306695
(6) Accuracy Score for Easy Ensemble Classifier:                      0.9197970678173006

### Confusion matrices for the six models are:

(1) Logistic regression w/RandomOverSampler
	                Predicted high_risk	  Predicted low_risk
Actual high_risk	        52  	                35
Actual low_risk	        5952	               11166

(2) Logistic regression w/SMOTE
	                Predicted high_risk	  Predicted low_risk
Actual high_risk	        56  	                31
Actual low_risk	        5840	               11278

(3) Logistic regression w/ClusterCentroids
	                Predicted high_risk	  Predicted low_risk
Actual high_risk	        52  	                35
Actual low_risk	        9684	                7434

(4) Logistic regression w/SMOTEENN
	                Predicted high_risk	  Predicted low_risk
Actual high_risk	        63  	                24
Actual low_risk	        7256	                9862

(5) Balanced Random Forest
	                Predicted high_risk	  Predicted low_risk
Actual high_risk	        58  	                29
Actual low_risk	        1560	               15558

(6) Easy Ensemble Classifier
	                Predicted high_risk	  Predicted low_risk
Actual high_risk	        78  	                 9
Actual low_risk	         975	               16143

### Imbalanced Classification Reports for the six models are:

(1) Logistic regression w/RandomOverSampler
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.60      0.65      0.02      0.62      0.39        87
   low_risk       1.00      0.65      0.60      0.79      0.62      0.39     17118

avg / total       0.99      0.65      0.60      0.78      0.62      0.39     17205

(2) Logistic regression w/SMOTE
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.64      0.66      0.02      0.65      0.42        87
   low_risk       1.00      0.66      0.64      0.79      0.65      0.42     17118

avg / total       0.99      0.66      0.64      0.79      0.65      0.42     17205

(3) Logistic regression w/ClusterCentroids
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.60      0.43      0.01      0.51      0.26        87
   low_risk       1.00      0.43      0.60      0.60      0.51      0.26     17118

avg / total       0.99      0.44      0.60      0.60      0.51      0.26     17205

(4) Logistic regression w/SMOTEENN
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.72      0.58      0.02      0.65      0.42        87
   low_risk       1.00      0.58      0.72      0.73      0.65      0.41     17118

avg / total       0.99      0.58      0.72      0.73      0.65      0.41     17205

(5) Balanced Random Forest
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.04      0.67      0.91      0.07      0.78      0.59        87
   low_risk       1.00      0.91      0.67      0.95      0.78      0.62     17118

avg / total       0.99      0.91      0.67      0.95      0.78      0.62     17205

(6) Easy Ensemble Classifier
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.07      0.90      0.94      0.14      0.92      0.84        87
   low_risk       1.00      0.94      0.90      0.97      0.92      0.85     17118

avg / total       0.99      0.94      0.90      0.97      0.92      0.85     17205



## Summary
