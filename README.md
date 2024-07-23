## Overview
This repository contains a Jupyter Notebook that details the process of training a neural network to predict student loan repayment success and provide a more accurate interest rate for the borrower. The project employs a dataset that includes various financial and demographic features to determine the likelihood of students successfully repaying their loans. The neural network model is built, evaluated, and used for predictions within the notebook.

## Requirements
To run this notebook, ensure you have the following installed:

- Python 3.8 or higher
- Jupyter Notebook or Google Colab
- TensorFlow 2.x
- Scikit-Learn
- Pandas
- Numpy

## Files in the Repository
- ***student_loans_with_deep_learning.ipynb:*** The main Jupyter Notebook file containing the neural network model's development and evaluation.
- ***student_loans.keras:*** The trained neural network model saved in Keras format.

## How to Use
1. **Preprocessing:** Data is split into features and target datasets. The target is the "credit_ranking" column, while the features include other demographic and financial data. The data is then split into training and testing sets. Feature data is scaled using Scikit-learn's StandardScaler.
2. **Compile and Evaluate the Model**: A deep neural network is created with 2 hidden layers suited to the data. The model is compiled using the Adam optimizer and accuracy metrics. After fitting the model with the training data over 50 epochs, its performance is evaluated on the test set.
3. **Predict Loan Repayment Success:** The trained model is saved and then reloaded. Predictions are made on the testing dataset. A classification report is generated to evaluate the predictions.

## Discussion on Recommendation Systems
The notebook concludes with a discussion on the potential for creating a recommendation system for student loans based on the insights and patterns learned from the data and model predictions.