# Term Deposit Prediction

## Introduction
In this project, I built a classification model to help call centers identify potential subscribers to a term deposit. Such a model has great practical value because call centers often waste a great amount of time speaking to people who will not subscribe, and the model can be a great filter to find the best possible clients. 

## Our Data
Our data is a year's worth of call center data from a European banking institution with the following data dictionary:

- **age** : age of customer (numeric)

 - **job** : type of job (categorical)

 - **marital** : marital status (categorical)

 - **education** (categorical)

 - **default**: has credit in default? (binary)

 - **balance**: average yearly balance, in euros (numeric)

 - **housing**: has a housing loan? (binary)

 - **loan**: has personal loan? (binary)

 - **contact**: contact communication type (categorical)

 - **day**: last contact day of the month (numeric)

 - **month**: last contact month of year (categorical)

 - **duration**: last contact duration, in seconds (numeric)

 - **campaign**: number of contacts performed during this campaign and for this client (numeric, includes last contact)

 - **y**: has the client subscribed to a term deposit? (our target binary variable)

## Methodology

After thorough data preprocessing and exploratory data analysis, I built a gradient boosting model using the low level api for the xgboost library. And with extensive feature engineering, data transformations, and SMOTE to reblance the target class, I trained my model with an early stopping callback to prevent over-fitting and achieved state of the art performance.
