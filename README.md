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

First, we created a neural network with just one hidden node that had twice the number of features as the input features. The first layer is the relu function and a sigmoid function. We obtained an accuracy of about 72.5% using a mean squared loss metric. Next we tried to add more layers to see if it would imporve the accuracy, but the accuracy we obtained was the same as before. Finally we tried to use a different loss metric to see if it would improve our accuracy. When running 100 epochs, we obtained an accuracy of 72.4%. And when running 300 epochs, we obtained an accuracy of 72.6%. 

To attain a better accuracy, we could look back at the dataframe and see if there are any other columns that can be dropped. This would hopefully streamline the data before it is processed through the neural networks. In addition, we could also to use a different learning model or a different loss metric to see if we can achieve better results. Running more epochs seemed to have boosted the accuracy by about 0.2%. However, we would not try to run more epochs in the future as it is time consuming.
