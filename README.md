# Neural_Networking

## Overview
In this Challenge we have been asked to build our own machine learning model to predict the success of a venture paid by Alphabet Soup.

### Resources
* Python 3.7, Scikit-learn 0.21, TensorFlow
* charity_data.csv

## Summary
### Preprocessing
We decided to drop the first two columns of the dataframe (EIN and NAME). This is because these are just used to identification columns. Next we created a categorical variable list and determined that the APPLICATION_TYPE and CLASSIFICATION columns needed to be buckted to streamline the data. Then we encoded the the categorical variable list and merged it with the dataframe. Finally we dropped the IS_SUCCESSFUL column from the dataframe, as it is going to be our target, and scaled the dataframe.

### Neural Networks

First, we created a neural network with just one hidden node that had twice the number of features as the input features. The first layer is the relu function and the 
