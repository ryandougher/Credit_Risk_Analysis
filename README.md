# Credit_Risk_Analysis

## Overview

The purpose of this project is to predict credit risk using credit card data. To predict credit risk, we first oversampled the data using the RandomOver Sampler and SMOTE algorithms. We then undersampled the data using the ClusterCentroids algorithm. Next, we used a combinatorial approach of over- and undersampling using the SMOTEEN algorithm. Lastly, we compared two machine learning models that reduce bias, BalancedRandomForestClassifer and EasyEnsembleClassifer, to predict credit risk.

## Results

The results of all six machine learning models can be seen below:

### Naive Random Oversampling

![Naive_Random_Oversampling](https://user-images.githubusercontent.com/96550846/171510040-efd696f1-a9f7-4d20-80f3-cfe43578a896.png)

- Balanced accuracy: 0.6497536370265621
- Precision: Low for high-risk loans, and high for low-risk loans
- Recall: High-risk / low-risk = 0.62 / 0.68

### SMOTE Oversampling

![SMOTE_oversampling](https://user-images.githubusercontent.com/96550846/171510758-809fa3fc-e648-4b10-affa-8bca0826e72c.png)

- Balanced accuracy: 0.6443721269403855
- Precision: Low for high-risk loans, and high for low-risk loans
- Recall: High-risk / low-risk = 0.63 / 0.66

### Undersampling

![Undersampling](https://user-images.githubusercontent.com/96550846/171510860-3a62fa5c-7e51-4c0b-b50d-101aae116593.png)

- Balanced accuracy: 0.6443721269403855
- Precision: Low for high-risk loans, and high for low-risk loans
- Recall: High-risk / low-risk = 0.60 / 0.43

### Combination Under-Overampling

![Combination_sampling](https://user-images.githubusercontent.com/96550846/171510990-c4cf8ee2-63bd-4d34-9656-4ad1ebc90f41.png)

- Balanced accuracy: 0.5158151733807124
- Precision: Low for high-risk loans, and high for low-risk loans
- Recall: High-risk / low-risk = 0.70 / 0.57

### Balanced Random Forest Classifier

![Random_forest_classifier](https://user-images.githubusercontent.com/96550846/171511060-9d1b223e-8d46-458e-b3ec-387bc939692e.png)

- Balanced accuracy: 0.7877672625306695
- Precision: Low for high-risk loans, and high for low-risk loans
- Recall: High-risk / low-risk = 0.67 / 0.91

### Easy Ensemble AdaBoost Classifier

![Easy_ensemble_adaboost](https://user-images.githubusercontent.com/96550846/171511166-80eb5601-d4fa-45a6-be3d-93bdd848b697.png)

- Balanced accuracy: 0.925427358175101
- Precision: Low for high-risk loans, and high for low-risk loans
- Recall: High-risk / low-risk = 0.91 / 0.94

## Summary

After reviewing all six models, the EasyEnsembleClassifier had the best results with an accuracy score of 0.925 and precision of 0.07 for high-risk. It also had the highest recall with 0.91 for high-risk and 0.94 for low-risk. The EasyEnsembleClassifier is the recommended model.

In order to improve the models, we recommend using a larger dataset for the high-risk category. The vast majority of the data was classified as low-risk, which can make it difficult to train the model to make predictions in the high-risk category.
