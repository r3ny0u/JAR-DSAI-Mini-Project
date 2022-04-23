# How to get richhh
## About
This is our SC1015 mini project which is on income taken from [Glassdoor- Analyze Gender Pay Gap](https://www.kaggle.com/datasets/nilimajauhari/glassdoor-analyze-gender-pay-gap), to predict income based on the various varibales. As a way to get rich.

## 1. [Data Extraction & explatory](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/data%20extraction%20%26%20explatory%20analysis.ipynb)
Extracing and visualise the dataset to gain insights. CLeaning the data to fit into our problem statement. Includes univariate analysis and mutlivariate analysis.

## 2. [Linear Regression](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/linear%20regression.ipynb)
[Train](https://github.com/r3ny0u/GetMeOut/blob/main/dataset/train.csv) 80% of the cleaned up dataset to predict income and using the remaining 20% to [test](https://github.com/r3ny0u/GetMeOut/blob/main/dataset/test.csv) the linear regression model. 1 model for only numerical variables and another model for all variables using one hot encoding(dummy) to fit in categorical data. 

## 3. [Resample]()
Wanting to test out tree classification model, we split the data into 2, '0' for below 75th percentile of income and '1' for above 75th percentile of income. Resulting in lesser '1' than '0'. Resample to prevent any biased data training.

## 4. [Tree Classifications](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/tree.ipynb)
Using different models of classification to find out which is the best model to predict income. 
### [Decision Tree Classification]()
### [Random Forest Classification]()
### [XGBoost]()

## 5. [Cross Validation](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/cross%20validation.ipynb)
To find the optimal tuning parameters for a machine learning problem. As we may encounter overfitting or underfitting which will reasult in higher levels of error when applied to our test. 

## Conclusion
Models are very accurate in predicting income but it might not be very accurate due to the small sample size of 1000. Accuracies for training models are a little too high which may symbolise some biasness. Could gather more similar datasets from other sources and combininig them together so as to better predict how we are able to get higher income.
