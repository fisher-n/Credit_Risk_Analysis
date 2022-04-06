# Credit_Risk_Analysis
## Analysis Overview
The purpose of this analysis is to use Python and data from LendingClub to build and evaluate machine learning models to predicts credit risk. 

## Results
### RandomOverSampler model
![This is an image](https://github.com/fisher-n/Credit_Risk_Analysis/blob/main/Resources/1.png)
![This is an image](https://github.com/fisher-n/Credit_Risk_Analysis/blob/main/Resources/2.png)
- The predicted accuracy score is 64%
- High risk precision is about 1% with a 62% sensitivity which makes a F1 of 2%

### SMOTE model
- The predicted accuracy score is 63%
- The high risk precision is about 1% with a 63% sensitivity which makes a F1 of 2%
- Due to the high number of low risk population, its precision is almost 100% with a 66% sensitivity.

### ClusterCentroids model
- The balanced accuracy score is 51%
- The high risk precsion is still 1% with a 63% sensitivity which makes a F1 1%
- Due to the high number of false positives, the low risk sensitivity is 40%

### SMOTEENN model
- The balanced accuracy is about 62%
- The high risk precision is 1% with 68% sensitivty with F1 of 2%
- Due to the high number of false positives, the low risk sensitivity is 57%

### BalancedRandomForestClassifier model
- The balanced accuracy score improved to 79%
- High risk percision is 4% and 67% sensitivity with F1 7%
- Due to a lower number of false positivies the low risk sensitivity is now 91% with 100% precision

### EasyEnsembleClassifier model
- Balanced accuracy score is 93%
- High risk precision is still love at 7% with 91% sensitivty which makes F1 14%
- Due to the lower number of false positives the low risk sensitivity is now 94% with 100% precision.

## Summary
The models showed that there is weak precision when the credit risk is high for this credit risk analysis. The ensemble models brought improvement to the sensitivity of high risk credits. The easyensembleclassifier model shows a recall of 92% so it detects almost all high risk credit. On another hand with a low precision, a lot of low risk credits are still falsey detected has high risk. This would penalize the bank's credit strategy and infer on its revenue by missing those bussiness opportunities. For these reasons I would not recommend the bank to use any of these models to predict credit risk
