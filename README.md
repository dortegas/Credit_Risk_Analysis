# Credit Risk Analysis

## Overview
Credit risk is an unbalanced classification problem, as good loans easily outnumber risky loans. For that reason, we employed different techniques to train and evaluate models with unbalanced classes like **imbalanced-learn** and **scikit-learn** libraries to build and evaluate models using resampling. For this challenge, we used the credit card credit dataset from LendingClub, a peer-to-peer lending services company, to oversample the data using the **RandomOverSampler** and **SMOTE** algorithms, and undersample the data using the **ClusterCentroids** algorithm. Then, we used a combinatorial approach of over-and undersampling using the **SMOTEENN** algorithm. Finally, we compared two new machine learning models that reduce bias: **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**, to predict credit risk.

## Results

<ins>**Oversampling**</ins>

- Naive Random Oversampling
<img src="Resources/model1.PNG" width="700">

- SMOTE Oversampling
<img src="Resources/model2.PNG" width="700">

**Undersampling**

- Cluster Centroids
<img src="Resources/model3.PNG" width="700">

- SMOTEENN Combination (Over and Under) Sampling
<img src="Resources/model4.PNG" width="700">

**Ensemble Learners**

- Balanced Random Forest Classifier
<img src="Resources/model5.PNG" width="700">

- Easy Ensemble AdaBoost Classifier
<img src="Resources/model6.PNG" width="700">

## Summary

    
