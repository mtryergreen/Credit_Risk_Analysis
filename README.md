# Credit_Risk_Analysis
## Objective
This project had me use Python to predict credit risk through machine learning models. I oversampled using RandomOverSampler and SMOTE algorithms and undersampled using ClusterCentroids algorithms. 

## Results
### Random OverSampler Model
Evaluations simlar to the one shown below were conducted with the various models. 
![Screen Shot 2022-03-01 at 3 16 21 PM](https://user-images.githubusercontent.com/89936913/156264955-6ae0ce2b-bdf4-470f-b6fb-6781ca0f6c17.png)
![Screen Shot 2022-03-01 at 3 18 21 PM](https://user-images.githubusercontent.com/89936913/156265163-0d18e0b0-a17d-40ff-96bc-e04ca811797a.png)

The balanced accuracy score is 68%, with high-risk precision at 1% with 62% sensitivity. 

### SMOTE Model
Balanced accuracy score is 64%. High risk precision is around 1% with 63% sensitivity so F1 is about 2%. 

### ClusterCentroids Model
Balanced score accuracy is down to 52%, and high risk precision is 1% with around 63% which makes F1 of 1%. Low risk sensitivity is around 40%. 

### SMOTEEN Model
Balanced accuraacy score is around 62%. High risk precision is 1% with 68% sensitivity which means F1 is around 2%. 
Low risk sensitivity is 57%. 

### BalancedRandomForestClassifier Model
Balanced accuracy score is about 79%. High risk precison is low at 4% with 67% sensitivity and F1 at 7%. Low risk sensitivity is 91% with 10% precision. 

### EasyEnsembleClassifier Model
Balanced accuracy score is 93%. High risk precision is at 7%, and 91% sensiticity and F1 at 14%. The low risk sensitivity is at 94% with 100% precision. 

# Summary
All models show show weak precision. Models like Ensemble had more responsiveness in terms of readings for high risk credits. Models like EasyEnsembleClassifier have high recall but also falsely detect a lot of low credit risks as high credit risks. Due to the inability for some models to differentiate between high and low risk, I would not recommend the bank to use any of the models to predict credit risk. 
