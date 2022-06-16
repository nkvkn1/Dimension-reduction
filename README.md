# Dimension-reduction
Explorint the basic forms of dimensionality reduction to prepare our data for training a AI or ML Model 


There are multiple ways of dimensionality reduction. In this file, I have used the famous wine dataset to demonstrate dimensionality reduction.

We go through the following 6 methods of dimension reduction:

1. MSV - Missing Value Ratio : In this method we look for the ratio of missing values in the dataset. If the missing values are a small ratio of the total data, we remove them. 

2. LVF - Low Variance Filter : In this, we filter out the features that do not vary much. By vary, I mean they do not change much. All the values in this column will be very close to each other. 

3. HCF - High correlation Filter : In this filter, we remove the features or columns that are highly correlated. We generally keep the one which has more correlation with the target variable. 

4. RF - Random Forest : We use Random forest from the sklearn library. We can get rid of the feature that has the least importance according to Random Forest.

5. BFE - Backward Feature Eliminiation : Backward Feature Elimination is also a part of sklearn library. In this approach, the model drops a feature at a time and then calculates the accuracy of a regressor. This regressor can be a linear regressor or a decision tree or so on. It checks the features that affect the regressor the most and keep the one that are important. You can select how many features you want to keep.

6. FFS - Forward feature selection : This is also a part of sklearn library. It is almost the opposite of BFE. In this approach, the model selects a feature and checks the accuracy of the regressor. it keeps on adding features and comparing the accuracy to each other. It does this till it select the desired amount of features. 
