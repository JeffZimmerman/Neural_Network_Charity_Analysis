# Neural Network Charity Analysis: A Neural Network Model

## Overview
This project used the TensorFlow platform in Python to develop and analyze a neural network for classifying charitable donations. The aim was to model training and testing data using machine learning to predict the success of these donations, to plan for best utilization of resources in the future.

## Results
* Data Preprocessing
Notable columns were identified and separated for preprocessing. The columns "EIN" and "NAME" were removed because they provided identification information irrelevant for modelling purposes. The target variable was the column "IS_SUCCESSFUL", based on results from previous allocations. The variables retained as features were "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", USE_CASE", "ORGANIZATION", "STATUS", INCOME_AMT", SPECIAL_CONSIDERATIONS", and "ASK_AMT."

* Compiling, Training, and Evaluating the Model
The initial model began with two hidden nodes, with 80 and 30 neurons, respectively. The activation functions for the nodes were ReLU and the output Sigmoid. This resulted in an accuracy of 73%. In the second attempt, a third node was added with a smaller number of neurons, so they were 80, 30, and 10, respectively. The activation functions for the nodes were kept as ReLU and the ouput as Sigmoid, but the accuracy decreased slightly to 67%. On the third attempt, the number of nodes and neurons remained the same as on the second attempt, but the activation function of the output was changed to tanh. The third attempt had markedly worse results, with an accuracy of only 47%.

## Summary
This neural network model was able to achieve a decent accuracy rating on the first attempt, but further actions taken in the name of optimization achieved worse results. This can be explained by an overfitting of the model to training data, and also by recognizing that the needs of an output layer are distinct from a hidden layer, so the tanh function is misplaced in the third attempt. To offset the risk of overfitting, experimenting with some additional attempts could suggest a better mix of number of nodes and nuerons. Adding more data to the training dataset could also be helpful if feasible. Notably, this modelling uses a large number of features, so thoughtfully reducing the number of these may offer the best hope for optimization. The accuracy rate of 73% on the first attempt may be adequate for low-stakes modelling, depending on the case, but this could be not much better than a more basic Supervised Machine Learning model such as Random Forest, which might offer a similar level of accuracy but with faster performance and less required computing power.
