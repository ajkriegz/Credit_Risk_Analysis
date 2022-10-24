# Credit_Risk_Analysis

This analysis was performed using Python 3, Jupyter Notebooks, and the imbalanced-learn and scikit-learn libraries.

## Overview

This analysis was performed to evaluate methods for assessing credit risk. The number of good loans heavily outnumbers risky loans, giving collected data unbalanced classes. Therefore, several techniques have been used and evaluated to assess the likely accuract of their predictions. 


## Results

The following terms important for understanding the data:

```Precision (pre): a measure of the number of true positives divided by the number of predicted positives. This number shows how reliable a positive classification is.```

```Recall / Sensitivity (rec): a measure of the number of true positives out of all true results. This number shows how well a model detects its intended targets.```

```Harmonic Mean (f1): a measure of the weighted mean that shows the balance between precision and sensitivity of a given model.```

```Balanced Accuracy: a measure of both the correct positives and negatives that shows how well a logistic regression model predicts results.```

For this analysis, the indicator to watch is high sensitivity scores for high risk applications as the goal is to correctly identify fraudulent applications, even at risk of false positives.

For the following lists, the first image will show the balanced accuracy score and the second image will show a report containing precision and recall scores.

---


* Naive Random Oversampling

![alt text][naive_acc]
![alt text][naive_rec]

This method's balanced accuracy score is neither the highest nor lowest of the methods at 0.668. Sensitivity to high risk applications is tied for second among the datasets at 0.70.

---


* SMOTE Oversampling

![alt text][smote_acc]
![alt text][smote_rec]

This method's balanced accuracy score is neither the highest nor lowest of the methods at 0.663. However, this method had the lowest sensitivity to high risk applications out of all six methods.

---

* ClusterCentroids Undersampling

![alt text][cc_acc]
![alt text][cc_rec]

This method's balanced accuracy score is neither the highest nor lowest of the methods at 0.663.Sensitivity to high risk applications is almost seven out of ten.

---

* Combination Sampling

![alt text][combo_acc]
![alt text][combo_rec]

This method has a low balanced accuracy score but a very high recall score, correctly identifying almost three out of four high risk applications. This method has the highest sensitivity to high risk applications out of all six methods.

---

* Random Forest Ensemble

![alt text][rf_acc]
![alt text][rf_rec]

This dataset is one of two with a very high balanced accuracy score of 0.789, showing that the model is very accurate at both predicting true positive and true negative results. Sensitivity to high risk applications is tied for second among the datasets at 0.70. While not the main focus, this method is tied for highest precision on high risk applications and is also tied for highest harmonic mean, showing itself to be slightly more balanced than the other tests.

---

* AdaBoost Ensemble

![alt text][ada_acc]
![alt text][ada_rec]

This dataset is one of two with a very high balanced accuracy score of 0.789, showing that the model is very accurate at both predicting true positive and true negative results. Sensitivity to high risk applications is tied for second among the datasets at 0.70. While not the main focus, this method is tied for highest precision on high risk applications and is also tied for highest harmonic mean, showing itself to be slightly more balanced than the other tests.


## Summary

The methods that stand out for this dataset are SMOTEENN combination sampling, Random Forest ensemble sampling, and Adaptive Boosting ensemble sampling. SMOTEENN had a low balanced accuracy score but had the highest sensitivity for high risk applications, 0.74. This method is recommended for attaining the lowest number of high risk applications possible.

However, for a more balanced approach, the ensemble sampling methods stand above the rest. With high sensitivity for high risk applications of 0.70 and very high balanced accuracy scores, these methods are more accurate. These methods may catch risky applications, but they will approve a higher number of low risk applications accurately. The analysis team recommends ensemble sampling for this reason.

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