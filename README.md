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

 | ML Model | Accuracy Score | Precision | Recall | F1 |
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

### SMOTEENN

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/SMOTEENN.png)

### Balanced Random Forest Classifier

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/Random%20Forest.png)

### Easy Ensemble Adaboost Classifier

![webpage](https://github.com/diercz/Credit_Risk_Analysis/blob/main/Images/Adaboost.png)

## Summary

Within the financial industry, sensitivity is a more valuable metric than precision when anylizing risk and default rates for loan candidates.  Banks need to be able to identify all high-risk loan candidates to ensure they do not select them and default on those loans.  

In terms of precision, all six algorithms had a really low precision rate for high risk individuals. The highest one was the Easy Ensemble AdaBoost Classifier with 7% precision which is still considered pretty low for finding these high risk individuals not to give loans to. This means that out of all the customers marked as high-risk 7% were actually high-risk. On the other hand, all the models had a perfect precision for low-risk individiauls meaning that all of the low-risk customers were marked as that.

Having this in mind, precision is not telling us much information to compare the algorithms, so we should take a look at sensitivity. The model with the highest sensitivity was the easy ensemble adaboost classifier (91% for high-risk and 94% for low-risk individuals), meaning that 91% of the time all the high-risk individuals are marked as high-risk individuals. Followed by this model, the other two with high recall were the Random Forest Classifier (67%) and SMOTEENN Resample (70%).

And last but not least, we are going to look at the balanced accuracy score to make the final decision of which model to use. The accuracy score stands for how correct was the model, meaning out of all the predictions how many of them were true to the classification. As we were able to see, the model with the highest accuracy score by far was the Easy Ensemble AdaBoost Classifier. So, this should be the one we chose because of its high accuracy, highest precision, and highest sensitivity.
