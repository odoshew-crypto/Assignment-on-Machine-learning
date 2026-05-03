-The goal of this project was to build a machine learning model that predicts whether a passenger survived the Titanic disaster. We used the Titanic dataset from Seaborn and applied data preprocessing, encoding, and classification models.

-The dataset was loaded using Seaborn:The dataset was loaded using Seaborn.
Some columns had missing values (e.g., age, embarked, deck).

-I handled them as follows:the values which were missing and a column which contained like 50% missing values:

Filled age with the median
Filled embarked with the most frequent value (mode)
Dropped deck due to too many missing values,,, 

-Machine learning models require numeric data, so we converted categorical columns:

sex: male → 0, female → 1
embarked: converted using one-hot encoding

-I split the dataset into training and testing sets:

80% training data
20% testing data

-I trained a Logistic Regression model after splitting it up there and evaluated it :
then also included the KNN  for comparision accuracy.

| Model               | Accuracy                  |
| ------------------- | ------------------------- |
| Logistic Regression | Higher / Good baseline    |
| KNN                 | Slightly lower or similar |
