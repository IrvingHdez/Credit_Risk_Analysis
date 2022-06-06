# Credit_Risk_Analysis

## Overview of the analysis: 
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. 
The idea is to employ different techniques to train and evaluate models with unbalanced classes.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 
Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results: 
### Re-Sampling Techniques:
* Naive Random Oversampling:
*imbalanced classification report*
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.02      0.71      0.86      0.05      0.78      0.60        87
   low_risk       1.00      0.86      0.71      0.92      0.78      0.62     17118

avg / total       0.99      0.86      0.71      0.92      0.78      0.62     17205

* SMOTE Oversampling
*imbalanced classification report*
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.03      0.71      0.88      0.06      0.79      0.62        87
   low_risk       1.00      0.88      0.71      0.94      0.79      0.64     17118

avg / total       0.99      0.88      0.71      0.93      0.79      0.64     17205

* Undersampling
*imbalanced classification report*
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.02      0.78      0.77      0.03      0.77      0.60        87
   low_risk       1.00      0.77      0.78      0.87      0.77      0.60     17118

avg / total       0.99      0.77      0.78      0.86      0.77      0.60     17205

* Combination (Over and Under) Sampling
*imbalanced classification report*
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.03      0.72      0.87      0.05      0.79      0.62        87
   low_risk       1.00      0.87      0.72      0.93      0.79      0.64     17118

avg / total       0.99      0.87      0.72      0.93      0.79      0.64     17205

## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.