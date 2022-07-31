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
![oversampling-naive](https://user-images.githubusercontent.com/102266450/182004197-c08309dd-ada2-4e91-8078-8f404faa188e.gif)
#### SMOTE: 
![oversampling-SMOTE](https://user-images.githubusercontent.com/102266450/182004203-d40a75bf-ca6d-442f-90a1-cd0bb3f374d6.gif)
### Undersampling Technique: 
#### ClusterCentroids: 
![undersampling-CC](https://user-images.githubusercontent.com/102266450/182004207-a9b8d903-b86a-45aa-baca-0a8d98697d48.gif)

## D2: SMOTEENN Algo to Predict (Credit Risk) 
![combo-SMOTE EEN](https://user-images.githubusercontent.com/102266450/182004215-b79c6514-3a00-4e50-839e-d619c327a2a8.gif)

## D3: Ensemble Classifiers to Predict (Credit Risk)
#### Balanced Random Forest Classifier:
![BRFC model](https://user-images.githubusercontent.com/102266450/182004232-8c05240a-45f3-4537-82e4-dc2fc3c59ad4.gif)

#### Easy Ensemble Classfier: 
![EEC model](https://user-images.githubusercontent.com/102266450/182004230-0460d7dc-fda8-4417-89d7-e14c13c37c9b.gif)

## Recommendations/Parting-Thoughts: 
If we focus on the balanced accuracy scores for each, we want to stay closest to 1 (0-1 range); and clealry our BRFC and EEC models fair the best. However, this is specific to this dataset, and we do not want to assume that replication for another dataset would yield the same results. 
With that said, we are most confident in the .92 accuracy provided from the EEC model, and recommend this be used for the current credit loan data. 
A downside is that this EEC model took nearly five minutes to run---a callout to the weak learner models from before, perhaps not as useful in its balanced accuracy scores, but much faster in runtime. 
We also observed precision and recall scores, and are once again confident in the EEC model. 
