# Telco Customer Churn Prediction using Neural Networks

## Overview

This repository contains code for predicting customer churn in a telecommunications dataset using a neural network implemented in TensorFlow and Keras. The dataset used is named "WA_Fn-UseC_-Telco-Customer-Churn.csv."

## Contents
### Data Loading and Preprocessing:

The dataset is loaded using Pandas, and initial exploratory data analysis is performed.
The 'customerID' column is dropped as it does not contribute to the prediction.
Missing values in the 'TotalCharges' column are handled.

### Data Visualization:

The distribution of customer tenure is visualized for both churn and non-churn groups using a histogram.

### Data Cleaning:

Some categorical values are standardized to maintain consistency and ease of processing.
Data Transformation:

Categorical variables are converted into numerical format (binary encoding) for model compatibility.
The 'gender' column is binarized (Male: 0, Female: 1).
Dummy variables are created for categorical features like 'InternetService,' 'Contract,' and 'PaymentMethod.'
Data Scaling:

The numerical features ('tenure,' 'MonthlyCharges,' 'TotalCharges') are scaled using Min-Max scaling.

### Model Training:

The dataset is split into training and testing sets using a standard 80-20 split.
A neural network model is defined with multiple layers and specified activation functions.
Binary crossentropy loss and the Adam optimizer are used during compilation.
The model is trained on the training data for 1000 epochs.

### Model Evaluation:

Model performance is assessed on the testing data.
### Dependencies
TensorFlow,
Keras,
NumPy,
Pandas,
Matplotlib,
Scikit-learn
