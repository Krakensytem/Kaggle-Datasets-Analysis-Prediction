# Kaggle-Datasets-Analysis-and-Prediction
This jupyter notebook implement, on a small scale, a ML solution, starting from reading and preparing the data, to performing the classification and evaluating the result. The attached data, which is available on [kaggle](https://www.kaggle.com/prakharrathi25/banking-dataset-marketing-targets), consists of several features describing both personal and financial attributes of an individual. Regarding the ML solution, it is implemented a binary classification to predict this classification. 

Below is presented the dataset analysis and prediction.

1.  #### Preparation and cleaning of data.
This consists of reading the data, search for missings and duplicates, and pre-processing it, to prepare the structure and data format required for the ingestion to the ML model. Regarding the Pearson Correlation coefficient was found there is no correlation, no relationship between the independent variables.

1. #### Processing, Visualisation and data analysis
It is presented a brief Data Exploration and Visualisation: A Bivariate analysis and plots of each feature by target Y (which specifies whether the individual proceeded with a “term deposit” or not). 
    * Categorical data: *job feature*: The bank contacted more on people with professional profiles. Most of the term deposit takers have a high qualification with regards to others.
    ![insert image here]().

    * Numerical data: *age feature*. This function shows the relationship between "age" and the categorical target variable using a box visual representations. Furthermore, the histogram displays a bell-shaped image, presents below, that has a left-shifted normal distribution. The population group is between 20 and 60. The box-plot shows an specific targeted age group between 30 and 50. Probably, because is when people are more productive and stable. This trend become stronger if we take into consideration the job feature. Bivariate analysis is great because it shows to the call center that they need to target a definite segment of customers.
    ![This is a alt text.](/image/sample.png "This is a sample image.")
    
1. #### Selecting the appropriate features 
Due to the cumbersome number of available attributes, it is applied some data analysis selecting the features which appear to be more significant than the rest. For this reason, noise is removed and encoding is performed.

1. #### Logistic Regression Model for Classification.
A logistic regression model is implemented in order to perform binary classification of each instance, as to whether or not a term deposit will happen. Confusion_matrix, classification report, cross validation mean and ROC and AUC are performed respectively.
.

1. #### Logistic Regression model evaluation.
The resulting classifier is evaluated, with “accuracy” as the scoring metric.

1. #### Oversampling
This method simply duplicates existing samples of a minor class to overcome the imbalance problem.
