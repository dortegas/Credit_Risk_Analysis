# Credit Risk Analysis

## Overview
Credit risk is an unbalanced classification problem, as good loans easily outnumber risky loans. For that reason, we employed different techniques to train and evaluate models with unbalanced classes like **imbalanced-learn** and **scikit-learn** libraries to build and evaluate models using resampling. For this challenge, we used the credit card credit dataset from LendingClub, a peer-to-peer lending services company, to oversample the data using the **RandomOverSampler** and **SMOTE** algorithms, and undersample the data using the **ClusterCentroids** algorithm. Then, we used a combinatorial approach of over-and undersampling using the **SMOTEENN** algorithm. Finally, we compared two new machine learning models that reduce bias: **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**, to predict credit risk.

## Results

<ins>**Oversampling**</ins>

**Naive Random Oversampling**
- Model balanced accuracy: 64%
- **High Risk** - Precision: 1%, Recall: 69% 
- **Low Risk**  - Precision: 100%, Recall: 59%
<img src="Resources/model1.PNG" width="750">

**SMOTE Oversampling**
- Model balanced accuracy: 66%
- **High Risk** - Precision: 1%, Recall: 63% 
- **Low Risk**  - Precision: 100%, Recall: 69%
<img src="Resources/model2.PNG">

<ins>**Undersampling**</ins>

**Cluster Centroids**
- Model balanced accuracy: 54%
- **High Risk** - Precision: 1%, Recall: 69% 
- **Low Risk**  - Precision: 100%, Recall: 40%
<img src="Resources/model3.PNG">

**SMOTEENN Combination (Over and Under) Sampling**
- Model balanced accuracy: 54%
- **High Risk** - Precision: 1%, Recall: 76% 
- **Low Risk**  - Precision: 100%, Recall: 59%
<img src="Resources/model4.PNG">

<ins>**Ensemble Learners**</ins>

**Balanced Random Forest Classifier**
- Model balanced accuracy: 78%
- **High Risk** - Precision: 3%, Recall: 70% 
- **Low Risk**  - Precision: 100%, Recall: 87%
<img src="Resources/model5.PNG">

**Easy Ensemble AdaBoost Classifier**
- Model balanced accuracy: 93%
- **High Risk** - Precision: 9%, Recall: 92% 
- **Low Risk**  - Precision: 100%, Recall: 94%
<img src="Resources/model6.PNG">

## Summary

Ensemble Learners models demonstrated superior recall performance in high-risk credit decisions compared to the other models in the analysis. However, the Easy Ensemble AdaBoost Classifier models' results showcase low precision scores, making them potential liabilities in real-life situations. These models are unreliable in our intended tasks, so I would not recommend them for predicting credit risk.
