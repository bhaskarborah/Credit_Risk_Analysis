#   Credit-Risk-Analysis

## Overview of Project
Fastlending, a peer to peer lending company wants to use Machine Learning to predict credit risk. The company wants to identify the good candidates to loan, so that it can reduce the current loan default rates. It will also better the loan disposal and issuance process.

The objective of this project is to build and evaluate several Machine Learning models, to predict credit risk for Fastlending. Also, to evaluate the models to see how accurately they predict the data.

## Purpose

The required input credit card credit dataset is available in a Comma Separated Values (CSV) file from LendingClub, a peer-to-peer lending services company

The purpose of this project is to provide the below deliverables:

Deliverable 1: Use Resampling Models to Predict Credit Risk
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

## Results

## Use Resampling Models to Predict Credit Risk

Deliverable 1: Use Resampling Models to Predict Credit Risk

### Random Oversampler (Oversampling)

![Screen Shot 2021-08-27 at 11.59.06 AM](https://i.imgur.com/x2Bd9y0.png)

Above are the Balanced Accuracy Score, Confusion Matrix and Imbalanced Classification report, when the data is resampled using RandomOverSampler.

The accuracy score is 0.65 or 65%.
Here 0 is High Risk and 1 is Low Risk.
The high risk precision is 0.01 or 1%, sensitivity is 0.63 or 63% and F1 is 0.02 or 2%.
The low risk precision is 1 or 100%, sensitivity is 0.67 or 67%  and F1 is 0.80 or 80%

### SMOTE (Oversampling)

![Screen Shot 2021-08-27 at 12.08.07 PM](https://i.imgur.com/x8MX1yC.png)


Above are the Balanced Accuracy Score, Confusion Matrix and Imbalanced Classification report, when the data is resampled using SMOTE.

The accuracy score is 0.61 or 61%.
Here 0 is High Risk and 1 is Low Risk.
The high risk precision is 0.01 or 1%, sensitivity is 0.55 or 55% and F1 is 0.02 or 2%.
The low risk precision is 1 or 100%, sensitivity is 0.66 or 66%  and F1 is 0.80 or 80%

The predictions are similar to Random Oversampler

### Cluster Centroids (Undersampling)

![Screen Shot 2021-08-27 at 12.13.09 PM](https://i.imgur.com/b46Y3tv.png)


Above are the Balanced Accuracy Score, Confusion Matrix and Imbalanced Classification report, when the data is resampled using Cluster Centroids.

The accuracy score is 0.52 or 52%.
Here 0 is High Risk and 1 is Low Risk.
The high risk precision is 0.01 or 1%, sensitivity is 0.57 or 57% and F1 is 0.01 or 1%.
The low risk precision is 1 or 100%, sensitivity is 0.47 or 47%  and F1 is 0.63 or 63%


## Use the SMOTEENN Algorithm to Predict Credit Risk

Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

### SMOTEENN

![Screen Shot 2021-08-27 at 12.28.02 PM](https://i.imgur.com/CONJ8qY.png)


Above are the Balanced Accuracy Score, Confusion Matrix and Imbalanced Classification report, when the data is resampled using SMOTTEEN.

The accuracy score is 0.63 or 63%.
Here 0 is High Risk and 1 is Low Risk.
The high risk precision is 0.01 or 1%, sensitivity is 0.71 or 71% and F1 is 0.02 or 2%.
The low risk precision is 1 or 100%, sensitivity is 0.54 or 54%  and F1 is 0.70 or 70%

## Use Ensemble Classifiers to Predict Credit Risk

Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

### Balanced Random Forest Classifier

![Screen Shot 2021-08-27 at 12.37.39 PM](https://i.imgur.com/K1yjwNh.png)


Above are the Balanced Accuracy Score, Confusion Matrix and Imbalanced Classification report, using BalancedRandomForestClassifier.

The accuracy score is 0.79 or 79%.
Here 0 is High Risk and 1 is Low Risk.
The high risk precision is 0.04 or 4%, sensitivity is 0.67 or 67% and F1 is 0.07 or 7%.
The low risk precision is 1 or 100%, sensitivity is 0.91 or 91%  and F1 is 0.95 or 95%. The number of false positives has decreased.

### Easy Ensemble Adaboost Classifier

![Screen Shot 2021-08-27 at 12.51.01 PM](https://i.imgur.com/H45UwGj.png)


Above are the Balanced Accuracy Score, Confusion Matrix and Imbalanced Classification report, using EasyEnsembleClassifier.

The accuracy score is 0.93 or 93%.
Here 0 is High Risk and 1 is Low Risk.
The high risk precision is 0.07 or 7%, sensitivity is 0.91 or 91% and F1 is 0.14 or 14%.
The low risk precision is 1 or 100%, sensitivity is 0.94 or 94%  and F1 is 0.97 or 97%. The number of false positives has further decreased.


#   Credit-Risk-Analysis-Summary

It can be seen that all the models have very low precision for high risk credit/loan. This means that these models show weak precision in determining which credit risk is high. 
However the Easy Assemble Adaboost Classifier has the highest accuracy of 93%. For high risks, the sensitivity is 91%, which is high, and shows that this model can detect the high risk credits. However the precision is still very low for high risks. However the precision is good for detecting low risk credits.
Of all these models, Easy Assemble Adaboost Classifier seems to be the most feasible to be used for Credit Risk Analysis, although it has the shortcoming of a low precision for high risks.






