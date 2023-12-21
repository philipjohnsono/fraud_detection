## Anomaly detection of fraud in credit card transactions 

### Introduction
The primary objective of this project is to identify instances of fraud in credit card transactions. By leveraging analytical techniques, I delve into the intricacies of transaction data to pinpoint anomalous patterns indicative of potential fraudulent activity. I employs multi-faceted approach to model creation, incorporating 3 machine learning algorithms: logistic regression, random forest, and support vector machine. In the case of the random forest, GridSearchCV was used in tuning the hyperparameter due to overfitting. Regarding the support vector machine, I increase the value of **C** and reduce the value of **gamma** due to overfitting.

### Data Sources Description
I used a credit card transactions dataset made by European cardholders in the year 2023 [link](https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023). It includes 568629 rows and 31 columns. The columns are namely; **id, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, V13, V14, V15, V16, V17, V18, V19, V20, V21, V22, V23, V24, V25, V26, V27, V28, Amount, Class**. Where **id** is the unique identifier for each transaction, **V1-V28** are the anonymized features representing various transaction attributes (e.g., time, location, etc.), **Amount** is the transaction amount in dollars, and **Class** is the a binary label specifying whether the transaction is fraudulent if the value is 1 and authorized when the value is 0. <br>

To safeguard cardholders' identities, data has been anonymized to uphold data privacy standards. <br>

Regarding bias and credibility, the data in question is sourced from the public domain kaggle. The information is deemed reliable, original, and up-to-date due to regular updates. Moreover, it is comprehensive, as it includes all important information necessary for the analysis, and was gathered in an ethical manner.

### Technologies
Python 3.5.0 <br>
Libraries: numpy, pandas, scikit-learn, seaborn and matplotlib.
