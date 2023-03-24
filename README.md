# Neural_Network_Charity_Analysis

## Overview

The goal of this project is to build a machine learning model to predict whether charities will be successful in receiving donations based on various factors such as application type, classification, and income amount. To achieve this, we used a deep learning neural network model.

In addition to the neural network model, we also performed data preprocessing which included binning and one-hot encoding.

# Results

## Data Preprocessing

What variable(s) are considered the target(s) for your model? 
The target variable for our model is the IS_SUCCESSFUL column, which indicates whether a charity was successful in receiving donations or not.

What variable(s) are considered to be the features for your model?
The features for our model are all columns except for IS_SUCCESSFUL, EIN, and NAME.

What variable(s) are neither targets nor features, and should be removed from the input data?
The EIN and NAME columns were removed from the input data as they were not useful for the model.

## Compiling, Training, and Evaluating the Model

For the initial neural network model, we used two hidden layers with 80 and 30 neurons respectively, and ReLU activation function.
For the optimized neural network model, we used four hidden layers with 80, 30, 20, and 10 neurons respectively, and ReLU activation function.
Both models used a binary crossentropy loss function and Adam optimizer, and were trained on 15 epochs.
The initial model achieved an accuracy of 72.9% on the test data, while the optimized model achieved an accuracy of 72.6%.
Although the optimized model did not significantly improve the accuracy, it may be able to generalize better to new data.

## Summary

In summary, we built a deep learning neural network model to predict whether charities will be successful in receiving donations. We performed data preprocessing using binning and one-hot encoding, and trained and evaluated the model using a variety of configurations. Despite our efforts to optimize the model, we were not able to achieve our target model performance of 75%. Therefore, we recommend exploring other machine learning models such as a random forest or support vector machine to solve this classification problem.
