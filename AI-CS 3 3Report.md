<a name="br1"></a> 

ASSIGNMENT 3 AI\_CS

Hadeer Mohamed

UOTTAWA 300327273



<a name="br2"></a> 

**Part I:**

**Exploratory Data Analysis (EDA):**

•

**Data Information:**

•

**Data Description**

•

**String Columns:**



<a name="br3"></a> 

**Data cleaning:**

**String columns is converted to integers**

•

•

**Check Skewness of the features**

•

**Check there is no null values**

•

**Count the Target Attacks**



<a name="br4"></a> 

•

**Correlation between attributes**

**Feature Selection using filter selection:**

• **Mutual\_Info filter method:**

o max mutal 82.20307370934049

o Best value of n components: 13

o ['FQDN\_count', 'subdomain\_length', 'lower', 'numeric', 'entropy', 'special', 'labels',

'labels\_max', 'labels\_average', 'longest\_word', 'sld', 'len', 'subdomain']

• **Chi2 filter method:**

o max chi2 82.20307370934049

o Best value of n components: 8

o **Best features**: ['FQDN\_count', 'subdomain\_length', 'upper', 'lower', 'numeric',

'special', 'labels', 'sld']

**Mutual\_Info filter method**

**Chi2 filter method**



<a name="br5"></a> 

**Model Training and Evaluation:**

**Decision Tree with Feature selection**

**Decision Tree after hyperparameter tuning:**

**Logistic Regression:**

**Logistic regression with hyperparameter tuning:**



<a name="br6"></a> 

The used Evaluation metric is **Accuracy** since the target data is approximately balanced

I used decision tree and logistic regression models it appears that decision tree (83.02) shows higher

accuracy than logistic regression (82%) so I choose Decision tree as the champion model and perform

hyperparameter tuning for DT in order to find the best hyperparameter and the result that the default

DT’s hyperparameter are the best.

**Cross\_Validatio for Decision tree model:**

Accuracy: 0.83 (+/- 0.01)

K-fold cross validation score: fo each

[0.81947035 0.82954122 0.83215218

0\.82879523 0.81797837 0.82767624

0\.82245431 0.8261194 0.83022388

0\.82052239]

**Part II (Dynamic Model):**

**Dynamic model (84.8%)** got slightly

higher accuracy than **static model (84.4%)**

