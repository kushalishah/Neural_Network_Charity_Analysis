# Neural_Network_Charity_Analysis

## Overview of Project
From Alphabet Soup’s business team, I received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. I used the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. I performed this task by creating a neural network by using data preprocessing, compiling, training and evaluating the model.

## Results

#### Data Preprocessing

For this analysis and model, the target is held in the IS_SUCCESSFUL field.

The following variables were considered as features for the model:
* ORGANIZATION
* STATUS
* INCOME_AMT
* SPECIAL_CONSIDERATIONS
* ASK_AMT
* APPLICATION_TYPE
* AFFILIATION
* CLASSIFICATION
* USE_CASE

The following variables were removed from the input and data:
* NAME
* EIN

#### Compiling, Training, and Evaluating the Model

**Model Configuration:**
The model was defined with the following features and hidden nodes for each layer:
* number_input_features = 43
* hidden_nodes_layer1 = 80
* hidden_nodes_layer2 = 30

The image below confirms the accuracy obtained from this model:
![d2_evaluate](https://github.com/kushalishah/Neural_Network_Charity_Analysis/blob/main/Images/d2_evaluate.png)

I made three attempts to optimize the model by trying to increase it's predictive accuracy to over 75%, in order to increase the model's performance.

Attempt 1:
![attempt1](https://github.com/kushalishah/Neural_Network_Charity_Analysis/blob/main/Images/attempt1.png)

Attempt 2:
![attempt2](https://github.com/kushalishah/Neural_Network_Charity_Analysis/blob/main/Images/attempt2.png)

Attempt 3:
![attempt3](https://github.com/kushalishah/Neural_Network_Charity_Analysis/blob/main/Images/attempt3.png)

This model achieved about 73% accuracy by increasing the features, activation functions, hidden layers, and the number of neurons in order to achieve this.

## Summary
From the results shown above, we can see that we weren't too far off with our target predictive accuracy of 75%. All three attempts resulted in a 73% accuracy. Perhaps, one recommendation would've been to change the activation functions such as: linear, tanh, sigmoid or a combination of these hidden layers. Or maybe, finding better features.
