# Neural_Network_Charity_Analysis

# Overview:
From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns,
APPLICATION_TYPE—Alphabet Soup application type,
AFFILIATION—Affiliated sector of industry,
CLASSIFICATION—Government organization classification,
USE_CASE—Use case for funding,
ORGANIZATION—Organization type,
STATUS—Active status,
INCOME_AMT—Income classification,
SPECIAL_CONSIDERATIONS—Special consideration for application,
ASK_AMT—Funding amount requested,
IS_SUCCESSFUL—Was the money used effectively.

We are using features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

# Data Preprocessing
# What variable(s) are considered the target(s) for your model?

The target variable considered for the model is "IS_SUCCESSFUL".

# What variable(s) are considered to be the features for your model?

The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT columns are considered to be the features of model. 

# What variable(s) are neither targets nor features, and should be removed from the input data?

The EIN, NAME, STATUS, and SPECIAL_CONSIDERATION columns are neither targets nor features and are removed from dataset by dropping the columns.

<img width="646" alt="features" src="https://user-images.githubusercontent.com/86980240/148703449-999d258e-f52a-48d5-98ee-671e61e0001d.png">


# Compiling, Training, and Evaluating the Model
# How many neurons, layers, and activation functions did you select for your neural network model, and why?

I selected 3 layers, 120 neurons with a sigmoid function for first layer, 80 nuerons with a ReLU function for the second, and 30 neurons for the third with ReLu and a sigmoid function for the outer layer. I changed the activation function for the first layer because it increased the model's performance.

<img width="628" alt="Neurons" src="https://user-images.githubusercontent.com/86980240/148703612-29803998-de20-429f-83b1-a7e49953e7e7.png">

# Were you able to achieve the target model performance?

Using TensorFlow, optimizing model in order to achieve a target predictive accuracy higher than 75%. I was able to achieve 73% with loss metrics of 0.5789

<img width="433" alt="accuracy" src="https://user-images.githubusercontent.com/86980240/148703773-9d5f6023-893d-47fa-a20e-08b343f4873b.png">

# What steps did you take to try and increase model performance?

I tried to boost performance by dropping few more columns, created more bins for rare occurrences in columns, increased the bin size. Then added another hidden layer and more neurons, used different activation functions for the hidden layers, increased the number of epochs.

# Summary

After removing unnecessary features, adding layers and neurons, increasing bins and changing activation function, the prediction accuracy of whether applicants will be successful if funded by Alphabet Soup was 73% and metric loss was 0.5789

# Recommendation

We can use a supervised machine learning model such as the Random Forest Classifier by randomly sampling the preprocessed data and building several decision trees. It is useful in case of overfitting the data, outliers and non linear data.



