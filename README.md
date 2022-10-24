# Credit_Risk_Analysis

This analysis was performed using Python 3, Jupyter Notebooks, and the imbalanced-learn and scikit-learn libraries.

## Overview

This analysis was performed to evaluate methods for assessing credit risk. The number of good loans heavily outnumbers risky loans, giving collected data unbalanced classes. Therefore, several techniques have been used and evaluated to assess the likely accuract of their predictions. 

## Results

* Naive Random Oversampling
![alt text][naive_acc]
![alt text][naive_rec]

* SMOTE Oversampling
![alt text][smote_acc]
![alt text][smote_rec]

* ClusterCentroids Undersampling
![alt text][cc_acc]
![alt text][cc_rec]

* Combination Sampling
![alt text][combo_acc]
![alt text][combo_rec]

* Random Forest Ensemble
![alt text][rf_acc]
![alt text][rf_rec]

* AdaBoost Ensemble
![alt text][ada_acc]
![alt text][ada_rec]


Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

## Summary

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

[naive_acc]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/naive_acc.png "Naive Balanced Accuracy Score"

[naive_rec]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/naive_recall.png "Naive Precision and Recall Scores"

[smote_acc]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/SMOTE_acc.png "SMOTE Balanced Accuracy Score"

[smote_rec]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/SMOTE_recall.png "SMOTE Precision and Recall Scores"

[cc_acc]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/cc_acc.png "ClusterCentroids Balanced Accuracy Score"

[cc_rec]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/cc_recall.png "ClusterCentroids Precision and Recall Scores"

[combo_acc]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_acc.png "SMOTEENN Balanced Accuracy Score"

[combo_rec]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_recall.png "SMOTEENN Precision and Recall Scores"

[rf_acc]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/rf_acc.png "Random Forest Balanced Accuracy Score"

[rf_rec]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/rf_recall.png "Random Forest Precision and Recall Scores"

[ada_acc]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/ee_acc.png "AdaBoost Balanced Accuracy Score"

[ada_rec]: https://github.com/ajkriegz/Credit_Risk_Analysis/blob/main/Resources/ee_recall.png "AdaBoost Precision and Recall Scores"