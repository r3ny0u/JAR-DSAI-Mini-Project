# How to get richhh
## About
This is our SC1015 mini project which is on income taken from [Glassdoor- Analyze Gender Pay Gap](https://www.kaggle.com/datasets/nilimajauhari/glassdoor-analyze-gender-pay-gap), to predict income based on the various varibales. As a way to get rich.

## 1. [Data Extraction & Explatory](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/data%20extraction%20%26%20explatory%20analysis.ipynb)
Extracing and visualise the dataset to gain insights. CLeaning the data to fit into our problem statement. Includes univariate analysis and mutlivariate analysis.

## 2. [Linear Regression](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/linear%20regression.ipynb)
[Train](https://github.com/r3ny0u/GetMeOut/blob/main/dataset/train.csv) 80% of the cleaned up dataset to predict income and using the remaining 20% to [test](https://github.com/r3ny0u/GetMeOut/blob/main/dataset/test.csv) the linear regression model. 1 model for only numerical variables and another model for all variables using one hot encoding(dummy) to fit in categorical data. 
![image](https://user-images.githubusercontent.com/101868598/164953979-2fa1dbd3-46f2-4bf9-b084-caad101fe1d3.png)
Linear model with only numerical data has a explained variance of 0.58 is not significant and shows that it still can be improved. While linear model with bother numerical and categorical data has an explained variance of 0.85 which is a lot better than the linear regression without adding categorical data.

## 3. [Resample]()
Wanting to test out tree classification model, we split the data into 2, '0' for below 75th percentile of income and '1' for above 75th percentile of income. Resulting in lesser '1' than '0'. Resample to prevent any biased data training.

## 4. [Tree Classifications](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/tree.ipynb)
Using different models of classification to find out which is the best model to predict income.
#### [Decision Tree Classification]()
<img src="https://user-images.githubusercontent.com/101868598/164954420-342584a8-a20d-4d90-8795-9a2b8498ed30.png" width="800" height="400"> 

#### [Random Forest Classification]()
<img src="https://user-images.githubusercontent.com/101868598/164954150-0d9e682a-8d4f-4ea3-9006-76436a5688d5.png" width="400" height="400"> 

#### [XGBoost]()
<img src="https://user-images.githubusercontent.com/101868598/164954157-0bf706b2-b89a-49e1-a017-98aec60f2fe3.png" width="400" height="400"> 

We found that XGBoost's train dataset has the highest accuracy of 1.0 but Random Forest has the highest accuracy of 0.95 for test dataset. However, the differences  in accuracy between these 2 models is not very significant. Hence, using either one of them is able to accurately predict how we can get high income.

## 5. [Cross Validation](https://github.com/r3ny0u/GetMeOut/blob/main/MegaDepression/cross%20validation.ipynb)
To find the optimal tuning parameters for a machine learning problem. As we may encounter overfitting or underfitting which will result in higher levels of error when applied to our test. 

## Conclusion
Models are very accurate in predicting income but it might not be very accurate due to the small sample size of 1000. Accuracies for training models are a little too high which may symbolise some biasness. Could gather more similar datasets from other sources and combininig them together so as to better predict how we are able to get higher income.

## Contributors
- Aden Ong Yew @AdenOng
- Chang Chieh Hsiang @jason-701
- Chang Ren You @r3ny0u

## References
- https://www.kaggle.com/datasets/nilimajauhari/glassdoor-analyze-gender-pay-gap
- https://towardsdatascience.com/cross-validation-and-grid-search-efa64b127c1b
