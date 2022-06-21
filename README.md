# Credit_Risk_Analysis

# Overview:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this challenge, I will employ different techniques to train and evaluate models with unbalanced classes. After cleaning the dataset, I discovered that of the 68,817 entries, the ration of the low risk and high risk classes were very disproportional.

![Screen Shot 2022-06-21 at 12 44 40 AM](https://user-images.githubusercontent.com/95712234/174717976-fac39e58-f052-4a75-abec-e9834f777e2b.png)

Using Python, I used several machine learning models to predict credit risk:

#### For Oversampling:
RandomOverSampler
SMOTE

#### For Undersampling:
ClusterCentroids

#### For a combination of oversampling and undersampling:
SMOTEENN

#### Compared two maching learning models that reduce bias:
BalancedRandomForestClassifier
EasyEnsembleClassifier

The models were run and then evaluated for performance and accuracy at predicting credit risk.

# Results:

