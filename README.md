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


 -I worked with the Wine dataset from sklearn. The main goal was to reduce the dimensionality of the data using PCA and t-SNE, then compare the results and model performance using Logistic Regression.
 which  I loaded the dataset using sklearn.it contaoins different chemicals variaties.
-i separeted the loadedt dataset using features and performed standardization on it.
-using Pca to work on tje data
PCA Analysis
Explained Variance

I plotted the cumulative explained variance to understand how many components I should keep.

From the plot, I observed that most of the information is retained in the first few components. I decided to keep enough components that explain around 45% of the variance.

Training Logistic Regression

I trained a Logistic Regression model in two ways:

On the original dataset
On PCA-reduced data
Comparison of Accuracy

I found that:

The original data gave higher accuracy
The PCA data gave slightly lower but still good accuracy
PCA reduced complexity while maintaining performance
-went ahead and took a lok at it by visualizing it. The plot showed that some classes were separated, but there was still slight overlap between them
-Using tsne to work on the data also so that i can compare the outome.
I applied t-SNE with different perplexity values:
