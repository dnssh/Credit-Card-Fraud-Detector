# Credit Card Fraud Detector

### Exploratory Data Analysis
![Data Distribution Accounts](/Images/Data%20Distribution.JPG)

Performed preprocessing and data visualization for top fraud accounts.
Estimated the amount lost in reversed and multi-swipe transactions.
> Achieved an AUC of 0.727 for blind set (XGBoost).

Analysed performance of various classification models- 
- XGBoost Classifier
- RandomForest Classifier
- DecisionTree Classifier
- Logistic Regression
- SVC

### Top Fraud accounts 
![Top fraud accounts](/Images/top10Fraud.JPG)

## Model Analysis
Here XGBoost has the an relatively high accuracy in predicting fraud transactions for the test_set compared to the previous models. Random forests are bagged decision tree models that split on a subset of features on each split instead of using all the features at once. This helps in determining the best step forward at each iteration

Amongst all the models XGBoost Classifier has the best Area under Curve and therefore is the best model for analysing and predicting the fraud transactions.

However Random Forest Classifier also has reasonably similar test accuracy and AUC. Hence even Random Forest Classifier can be considered as a good choice for predicting the fraud transactions


Test Data Accuracies:

| Model | Accuracy |
| ------ | ------ |
| Support Vector Classifier | 0.5657 |
| Decision Tree Classifier | 0.5725 |
| Logistic Regression | 0.6434 |
| Random Forest | 0.6701 |
| XGBoost Classifier | 0.6704 |

![Top fraud accounts](/Images/Graph.JPG)

Based upon the AUC and above Confusion Matrix the choice of models for the Fraud prediction is as follows:
### XGBoost >= Random Forest > Logistic Regression > Decision Tree > SVC
The model accuracies can be improved with feature engineering and tuning the hyperparameters in future
Also we can use F1 score, rms error asa metric to evaluate.
