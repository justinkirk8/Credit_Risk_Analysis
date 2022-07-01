# Credit_Risk_Analysis

## Overview of Analysis:
Client requested the provided credit card risk data set to be analyized. The data is unbalanced due to a larger ammount of good loans outweighing the bad loans. Client requests the following models to be evaluated: Naive Random Sample, SMOTE Oversampling, ClusterCentroid Understampling, SMOTEENN Sampling, Balanced Random Forest Classifier, and Easy Ensemble AdaBooster Classefier. Data obtained from LendingClub. 

## Resources
- Source Data: LoanStats_2019Q1.csv
- Software: Python 3.10 (64-bit), Jupyter Notebook 6.4.8

## Results

### Naive Random Sample and Linear Regression

- Accuracy:              0.64
- Precision High Risk:   0.01
- Precision Low Risk:    1.00
- Recall High Risk:      0.69
- Recall Low Risk:       0.59

<p align = "left">
  <kbd><img src="https://github.com/justinkirk8/Credit_Risk_Analysis/blob/main/image/naive_random.png" width="600" /></kbd>
</p>

### SMOTE Oversampling and Linear Regression

- Accuracy:              0.66
- Precision High Risk:   0.01
- Precision Low Risk:    1.00
- Recall High Risk:      0.63
- Recall Low Risk:       0.69

<p align="left">
  <kbd><img src="https://github.com/justinkirk8/Credit_Risk_Analysis/blob/main/image/smote_oversampling.png" width="600" /></kbd>
</p>

### ClusterCentroids Understampling and Linear Regression

- Accuracy:              0.54
- Precision High Risk:   0.01
- Precision Low Risk:    1.00
- Recall High Risk:      0.69
- Recall Low Risk:       0.40

<p align="left">
  <kbd><img src="https://github.com/justinkirk8/Credit_Risk_Analysis/blob/main/image/ClusterCentroids.png" width="600" /></kbd>
</p>

### SMOTEENN Sampling and Linear Regression

- Accuracy:              0.67
- Precision High Risk:   0.01
- Precision Low Risk:    1.00
- Recall High Risk:      0.76
- Recall Low Risk:       0.59

<p align="left">
 <kbd> <img src="https://github.com/justinkirk8/Credit_Risk_Analysis/blob/main/image/smoteenn.png" width="600" /></kbd>
</p>

### Balanced Random Forest Classifier

- Accuracy:              0.79
- Precision High Risk:   0.03
- Precision Low Risk:    1.00
- Recall High Risk:      0.70
- Recall Low Risk:       0.87

<p align="left">
  <kbd><img src="https://github.com/justinkirk8/Credit_Risk_Analysis/blob/main/image/random_forest.png" width="600" /></kbd>
</p>

### Easy Ensemble AdaBooster Classifier

- Accuracy:              0.93
- Precision High Risk:   0.09
- Precision Low Risk:    1.00
- Recall High Risk:      0.92
- Recall Low Risk:       0.94

<p align="left">
  <kbd><img src="https://github.com/justinkirk8/Credit_Risk_Analysis/blob/main/image/AdaBooster.png" width="600" /></kbd>
</p>

## Summary

Of the first four models, the precision was the same. SMOTE possessed the best Recall and F1 score while SMOTEENN possessed the best Accuracy and Accuracy and Specificity. The Balanced Random Forest Classifier showed an increase in almost every metric over the first four models. The only exceptions being low risk Specificity and high risk Recall. The final model, Easy Ensemble AdaBooster Classifier, shows a significant increased in every metric. Most importantly, it increases high risk Precision from 0.03 to 0.09. Of these models, I would highly recommend using the Easy Ensemble AdaBooster Classifier. However, I would continue to test additonal models to see if a better precision score on high risk loans can be found. 

