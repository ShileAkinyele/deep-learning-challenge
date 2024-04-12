# deep-learning-challenge

#Purpose of The Analysis 
This Analysis tries to use Machine learning and Neural networks to create a  binary classifier that can predict whether applicants will be successful if funded by a non nonprofit foundation.

#Summary of the Analysis 
The target variable for the model is the IS_SUCCESSFUL? which represents if the the money was used successfuly or not.
for the features variable such as APPLICATION_TYPE,AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT have been used.
The name and the EIN variables were droped from the input data as they are neither targets or features.

In other to compile and train the model, 43 input features were used which is the lenght of the X_train data, 2 hidden layers were used and an epoch of 100. for the first hidden layer, a total of 80 neurons were used and for the second hidden layer, 30 neurons were used.The units for the outer layer was 1 as its a binary classification problem, the result is either 1 or 0. The relu activation function was used for the two hidden layers while the sigmoid activation function was used for the outer layer.The relu function was used for the hidden layers as a standard function for hidden layers while sigmoid was used because we are trying to predict a probability.

In other to optimize the model, i tried using 4 hidden layers in the first instance and increasing the amount of neurons, also i used a different activation function for the first and second layer(tanh), also the epochs were reduced to 40
In the second instance of optimization, i try using 5 hidden layers, and an epoch of 50
in the third instance i try using 3 hidden layers and an epoch of 100, all of these optimization processes didnt meet the target.

The model before optimization was able to predict 72.51% Accuracy while the first attempt of optimization was able to predict 72.65% Accuracy.
