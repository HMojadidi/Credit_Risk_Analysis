# Credit_Risk_Analysis

# Overview:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this challenge, I will employ different techniques to train and evaluate models with unbalanced classes. After cleaning the dataset, I discovered that of the 68,817 entries, the ration of the low risk and high risk classes were very disproportional.

![Screen Shot 2022-06-21 at 12 44 40 AM](https://user-images.githubusercontent.com/95712234/174717976-fac39e58-f052-4a75-abec-e9834f777e2b.png)

Using Python, I used several machine learning models to predict credit risk:

#### For Oversampling:
RandomOverSampler and SMOTE

#### For Undersampling:
ClusterCentroids

#### For a combination of oversampling and undersampling:
SMOTEENN

#### Compared two maching learning models that reduce bias:
BalancedRandomForestClassifier and EasyEnsembleClassifier

The models were run and then evaluated for performance and accuracy at predicting credit risk.

# Results:

## Naive Random Oversampling:

![Screen Shot 2022-06-21 at 1 09 56 AM](https://user-images.githubusercontent.com/95712234/174720736-0172ea13-5218-4374-84dc-292be134bf6b.png)

![Screen Shot 2022-06-21 at 1 10 30 AM](https://user-images.githubusercontent.com/95712234/174720793-361dc46b-f575-45b3-87fc-15c46fbe3124.png)


## SMOTE Oversampling:

![Screen Shot 2022-06-21 at 1 06 14 AM](https://user-images.githubusercontent.com/95712234/174720339-b4d0be05-f897-4f4f-b4a7-bc011522da1e.png)

![Screen Shot 2022-06-21 at 1 07 40 AM](https://user-images.githubusercontent.com/95712234/174720505-8e5e3a94-0c17-4a0f-8543-4c4a14c8261a.png)

## 
