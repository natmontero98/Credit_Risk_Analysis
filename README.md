# Credit_Risk_Analysis

## Overview of the analysis
The purpose of this analysis is to find the best machine learning model to predict the credit risk of a loan, by using the credit card dataset from LendingClub, a peer-to-peer lending services company.

## Results: 
After running each model, the measurements we'll use to evaluate and compare their performances are: balanced accuracy scores, precision, and recall scores.
The results for each model were the following:

### Random Oversampling
* balanced accuracy score: 0.65
* precision:  0.99 
* recall: 0.59
### SMOTE Oversampling
* balanced accuracy score: 0.62
* precision: 0.99
* recall: 0.66
### Cluster Centroids
* balanced accuracy score: 0.62
* precision: 0.99
* recall: 0.41
### SMOTEEN
* balanced accuracy score: 0.54
* precision: 0.99
* recall: 0.57
### BalancedRandomForestClassifier
* balanced accuracy score: 0.75
* precision: 0.99 
* recall: 0.86
### EasyEnsembleClassifier
* balanced accuracy score: 0.69
* precision: 1.00
* recall: 1.00

## Summary
According to the results of the models, balanced accuracy scores were very similar, they ranged from 0.54 to 0.75, being the Balanced Random Forest model the one with the highest score. The model with the second highest balanced accuracy score was the Easy Ensembler Classifier. It's important to note that both of this models are part of the Ensemble Classifiers method.

For the precision score, the results were almost exactly the same, they all got a score of 0.99, except for the Easy Ensemble Classifier model, with a precision score of 1.0. 

The largest difference in results appeared in the recall scores, which ranged from 0.41 to 1.00. The models with the highest scores were, once again, Ensemble Classifiers, with a score of 1.00 for the Easy Ensemble model and 0.86 for the Random Forest model. The model with the lowest recall score was the Cluster Centroids one. 

Given the mentioned results, the best models to use are the Easy Ensemble Classifier and the Balanced Random Forest Classifier. These both models consistently showed higher scores than the resampling models. 

We want to avoid false positives as much as posible, because missing a high risk credit and approving it wouldn't be beneficial for the company, so we should give priority to precision scores. The model with the highest precision score for 0/high-risk loans, is the Easy Ensemble Classifier, so that would be the recommendation for this case. 

<img width="653" alt="Captura de Pantalla 2021-10-17 a la(s) 23 13 42" src="https://user-images.githubusercontent.com/85467925/137668321-165c564a-c44e-4f1d-8334-f5e3a457ad0c.png">

