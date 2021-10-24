# Credit_Risk_Analysis

# Overview of the analysis

This analysis evaluates machine learning models for predicting credit card risk(High/Low) with unbalanced classes and try to recommend which model to use.
The models used are :-
* Naive Random Oversampling
* SMOTE Oversampling
* Undersampling 
* Combination Oversampling and Undersampling 
* Ensemble(Balanced Random Forest Classifier) 
* Easy Ensemble AdaBoost Classifier
Credit card credit dataset from LendingClub, a peer-to-peer lending services company, is used using imbalanced-learn and
scikit-learn libraries to build and evaluate models to predict credit risk and evaluate performance of the models.

# Results

* Naive Random Oversampling

The precision for prediction of high credit card risk is very low 0.01 and that of low credit card risk is equal to 1.00.
The recall (sensitivity) for predicting high credit card risk is 0.70 and for low credit card risk is 0.63.
F1 score for high credit card risk is 0.02 this is due to a very low precision value from high credit card (0.01).
Accuracy score equals 0.77 and is worst on predicting high credit card risk. 

![NaiveRandonOversampling](https://user-images.githubusercontent.com/86446609/138593697-785edeb9-6448-4e1e-a037-0b0d8fbee5b7.JPG)

* SMOTE Oversampling

The precision for prediction of high credit card risk is very low 0.01 and that of low credit card risk is equal to 1.00.
The recall (sensitivity) for predicting high credit card risk is 0.63 and that of low credit card risk is 0.69.
F1 score for high credit card risk is 0.02 this is due to a very low precision value from high credit card 0.01.
Accuracy score equals 0.81 and is worst on predicting high credit card risk. 

![SMOTEOversampling](https://user-images.githubusercontent.com/86446609/138593700-cff85b93-bd25-4341-bd0c-d9c6d2fd2e2c.JPG)

* Undersampling 

The precision for prediction of high credit card risk is very low 0.01 and that of low credit card risk is equal to 1.00.
The recall (sensitivity) for predicting high credit card risk is 0.69 and that of low credit card risk is 0.40.
F1 score for high credit card risk is 0.01 this is due to a very low precision value from high credit card 0.01.
Accuracy score equals 0.56 and shows worst on predicting both high and low credit card risk. 

![Undersampling](https://user-images.githubusercontent.com/86446609/138593705-7717aca1-1bb4-4b00-b350-088244960714.JPG)

* Combination Oversampling and Undersampling 

The precision for prediction of high credit card risk is very low 0.02 and that of low credit card risk is equal to 1.00.
The recall (sensitivity) for predicting high credit card risk is 0.72 and that of low credit card risk is 0.57.
F1 score for high credit card risk is 0.02 this is due to a very low precision value from high credit card 0.01.
F1 score for low credit card risk is 0.72 this is due to a low recall value from low credit card(0.57).
Accuracy score equals 0.72 and the algorithm is worst on predicting both high and low credit card risk. 

![CombinationOversamplingUndersampling](https://user-images.githubusercontent.com/86446609/138593708-89baade0-6523-4e9a-974e-210bd6ee29b1.JPG)

* Ensemble(Balanced Random Forest Classifier) 

The precision for prediction of high credit card risk is very low 0.03 and that of low credit card risk is equal to 1.00.
The recall (sensitivity) for predicting high credit card risk is 0.70 and 0.87 for low credit card risk.
F1 score for high credit card risk is 0.06 this is due to a very low precision value from high credit card(0.03).
Accuracy score equals 0.93 and the algorithm is best on predicting low credit card risk. 

![Ensemble](https://user-images.githubusercontent.com/86446609/138593715-bc42d556-49d8-46f4-82ad-7334e3a2ef05.JPG)

* Easy Ensemble AdaBoost Classifier

The precision for prediction of high credit card risk is very low 0.09 and that of low credit card risk is equal to 1.00.
The recall (sensitivity) for predicting high credit card risk is 0.92 and 0.94 for low credit card risk.
F1 score for high credit card risk is 0.16 this is due to a very low precision value from high credit card(0.09).
Accuracy score equals 0.97 and the algorithm is best on predicting low credit card risk. 

![EasyEnsemble](https://user-images.githubusercontent.com/86446609/138593720-fe630506-94de-4603-86e2-90b9a946521e.JPG)

# Summary

The precision and F1 score for high credit card rish show a very low figure on most cases. The recall shows a significant figure on
both high credit card risk and low credit card risk data.The accuracy figures reveals the data as correct on low credic card risks.
On analyzing credit card risk what is more important is to get accurate data on high credit card risks . the result clearly shows significant figures on predicting 
recall (sensitivity). For credit card risk It’s more important to detect potentially fraudulent transactions, so sensitivity is more important here.
Therefore, Easy Ensemble AdaBoost Classifier with recall value of 0.92 and 0.94 for high rish and low risk with accuracy score 0.97 is recomended to use.

