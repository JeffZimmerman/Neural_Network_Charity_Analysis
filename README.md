# Neural Network Charity Analysis: A Neural Network Model

## Overview
This project used the TensorFlow platform in Python to develop and analyze a neural network for classifying charitable donations. The aim was to model training and testing data using machine learning to predict the success of these donations, to plan for best utilization of resources in the future.

## Results
* Data Preprocessing
Notable columns were identified and separated for preprocessing. The columns "EIN" and "NAME" were removed because they provided identification information irrelevant for modelling purposes. The target variable was the column "IS_SUCCESSFUL", based on results from previous allocations. The variables retained as features were "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", USE_CASE", "ORGANIZATION", "STATUS", INCOME_AMT", SPECIAL_CONSIDERATIONS", and "ASK_AMT."

* Compiling, Training, and Evaluating the Model
The initial model began with two hidden nodes, with 80 and 30 neurons, respectively. The activation functions for the nodes were ReLU and the output Sigmoid. This resulted in an accuracy of 73%. In the second attempt, an additional hidden node was added to make three, with neurons of 110, 50, and 20. The activation functions for the nodes were kept as ReLU and the ouput as Sigmoid, but the accuracy decreased markedly to 53%. On the third attempt, 
## Summary
