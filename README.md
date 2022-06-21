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

The balanced accuracy score is 66%.
The high_risk precision is about 1% only with 69% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 62%.

## SMOTE Oversampling:

![Screen Shot 2022-06-21 at 1 06 14 AM](https://user-images.githubusercontent.com/95712234/174720339-b4d0be05-f897-4f4f-b4a7-bc011522da1e.png)

![Screen Shot 2022-06-21 at 1 07 40 AM](https://user-images.githubusercontent.com/95712234/174720505-8e5e3a94-0c17-4a0f-8543-4c4a14c8261a.png)

The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 60% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 67%.



## ClusterCentroids Undersampling:

![Screen Shot 2022-06-21 at 1 13 50 AM](https://user-images.githubusercontent.com/95712234/174721131-4e5db7f9-c39b-4069-ad7f-30a743122f6a.png)

![Screen Shot 2022-06-21 at 1 14 13 AM](https://user-images.githubusercontent.com/95712234/174721164-5c59b968-6c0b-48ec-baf0-745e2cbad1b3.png)

The balanced accuracy score is 53%.
The high_risk precision is about 1% only with 66% sensitivity which makes a F1 of 1% only.
Due to the high number of false positives, the low risk sensitivity is only 40%.

## SMOTEENN: Combination (Over and Under) Sampling:

![Screen Shot 2022-06-21 at 1 15 22 AM](https://user-images.githubusercontent.com/95712234/174721288-c2e9394e-9b3b-4eda-b396-fcf3c56ee10e.png)

![Screen Shot 2022-06-21 at 1 15 39 AM](https://user-images.githubusercontent.com/95712234/174721320-4f6756c6-1a6e-4c4c-8791-66d6fba95650.png)

The balanced accuracy score is about 65%.
The high_risk precision is still 1% only with 74% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 56%.


## Balanced Random Forest Classifier:

![Screen Shot 2022-06-21 at 1 19 07 AM](https://user-images.githubusercontent.com/95712234/174721721-911b6b49-0635-475c-b61f-a9c0fdd5a102.png)

![Screen Shot 2022-06-21 at 1 19 42 AM](https://user-images.githubusercontent.com/95712234/174721785-468ff4fe-ea1e-4d45-a41d-6fae75098bb8.png)

The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% precision.


## Easy Ensemble AdaBoost Classifier:


![Screen Shot 2022-06-21 at 1 22 27 AM](https://user-images.githubusercontent.com/95712234/174722136-01aa85d9-3ae5-45c1-abb7-d933b1fe0156.png)

![Screen Shot 2022-06-21 at 1 23 03 AM](https://user-images.githubusercontent.com/95712234/174722222-e54421f1-f5bb-4f75-a063-8e9b37df391c.png)

Here, the balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

