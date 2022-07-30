# Credit_Risk_Analysis
## Background:
### Initial Concerns: 
Through our given credit loans data, our point of contact on this project insists we leverage the "imbalanced-learn" and "scikit-learn" libraries to build and evaluate models via resampling techniques. 
At its core, the loan data measures credit risk for users. We are using machine learning to solve this challenge/risk, but thus far (pre-challenge) have seen weak learner models. 
### Next Steps: 
Our "LendingClub" dataset will go through an oversampling process using the "RandomOverSampler" and "SMOTE" algorithims. Then we also use the "ClusterCentroids" algorithim for undersampling. 
Finally, we will use "SMOTEENN" as a combination approach. 
Ultimately, our goal here is to compare the two new ML models that ideally reduce bias. Our classifiers will predict the credit risk/user and we will evaluate the models with our final print outs. 
## D1: Resampling Models to Predict (Credit Risk)
### First Steps: 
We are using the "LoanStats_2019Q1.csv" as our dataset. In this section, we want to determine which ML model is better at predicting credit risk (evaluation stage).
### General Process:
#### Train/Target Steps:
    1. Create training variables, convert string to numerical with get_dummies()
    2. Create target variables
    3. Check the balance of our target variables, before resampling
#### Resampling Data Steps: 
    1. Use logisticregression classifier to make predictions, evaulate performance of each model 
    2. Calculate the accuracy score of each model
    3. Generate the confusion matrix
    4. Print out the imbalanced classification report
### Oversampling Techniques:
#### RandomOverSampler:
#### SMOTE: 
### Undersampling Technique: 
#### ClusterCentroids: 
### Results:

## D2: SMOTEENN Algo to Predict (Credit Risk) 
### Results:
## D3: Ensemble Classifiers to Predict (Credit Risk)
#### Balanced Random Forest Classifier:
#### Easy Ensemble Classfier: 
### Results: