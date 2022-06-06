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
![one](https://github.com/IrvingHdez/Credit_Risk_Analysis/blob/main/images/1.PNG)

* SMOTE Oversampling
*imbalanced classification report*
![two](https://github.com/IrvingHdez/Credit_Risk_Analysis/blob/main/images/2.PNG)

* Undersampling
*imbalanced classification report*
![three](https://github.com/IrvingHdez/Credit_Risk_Analysis/blob/main/images/3.PNG)

* Combination (Over and Under) Sampling
*imbalanced classification report*
![four](https://github.com/IrvingHdez/Credit_Risk_Analysis/blob/main/images/4.PNG)

## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.