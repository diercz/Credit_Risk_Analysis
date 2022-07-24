# Credit_Risk_Analysis

*Utilized several machine learning models to predict credit risk using Python's imbalanced-learn and scikit-learn libraries*

## Supervised Machine Learning Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes.  We then will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Resources
 - Dataset
    - LoanStats_2019Q1.csv

- Software
    - Python
    - Jupyter Notebook
    - NumPy, Skikit-learn, & Imbalanced Libraries
    - Logistic Regression
    - Random Forest Models
    - Ensemble and resampling techniques

## Results 

Below are the results of all six machine learning algorithms.

 | ML Model | Balanced Accuracy Score | Precision | Recall | F1 |
 | --- | --- | --- | --- | --- |
 | Naive Random Oversampling | 0.64 | 0.99 | 0.68 | 0.80 |
 | SMOTE Oversampling | 0.64 | 0.99 | 0.63 | 0.77 |
 | Cluster Centroid Undersampling | 0.51 | 0.99 | 0.44 | 0.60 | 
 | SMOTEENN Combination Sampling | 0.63 | 0.99 | 0.57 | 0.73 |
 | Balanced Random Forest Classifier | 0.78 | 0.99 | 0.91 | 0.95 |
 | Easy Ensemble AdaBoost Classifier | 0.93 | 0.99 | 0.94 | 0.97 |
 
### Naive Random Oversampling

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/Naive%20Random%20Oversampling.png)

### SMOTE Oversampling

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Oversampling.png)

### Cluster Centroid Undersampling

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/Cluster%20Centroid.png)

### Balanced Random Forest Classifier

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/Random%20Forest.png)

### Easy Ensemble Adaboost Classifier

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/Adaboost.png)