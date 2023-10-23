# Credit Card Fraud Detection

This Python script is designed to perform credit card fraud detection using a Decision Tree Classifier. The dataset used is read from a CSV file named "credit card.csv" using the Pandas library.

## Prerequisites

Before running this script, make sure you have the following Python libraries installed:
- pandas
- numpy
- plotly
- scikit-learn

You can install these libraries using pip:
  pip install pandas numpy plotly scikit-learn


# Usage
Data Loading: The script reads the credit card transaction data from the "credit card.csv" file using Pandas and displays the first few rows and the count of missing values.

Data Visualization: It visualizes the distribution of transaction types using a Pie Chart created with Plotly. This chart shows the percentage distribution of different transaction types.

Data Preprocessing: It preprocesses the data by mapping the "type" and "isFraud" columns to numeric values for machine learning. It assigns numeric values to transaction types and converts "isFraud" to "No Fraud" or "Fraud".

Machine Learning: The script uses a Decision Tree Classifier from scikit-learn to build a machine learning model for fraud detection. It splits the dataset into training and testing sets and trains the model using the training data.

Model Evaluation: The accuracy score of the model on the test data is printed to evaluate its performance.


# Customize
You can customize this script for your specific use case by modifying the following parts:

Input Data: Replace "credit card.csv" with your dataset's filename or path.

Feature Selection: You can change the features used for training the model by modifying the x array. Make sure the feature columns in the dataset match the features in the x array.

Target Variable: If your dataset uses different labels for fraud and no fraud (e.g., 1 for fraud and 0 for no fraud), modify the mapping in the "isFraud" column accordingly.

Model Selection: If you want to use a different machine learning model, replace the Decision Tree Classifier with your desired model from scikit-learn.

Test Size: You can adjust the test size when splitting the data by changing the test_size parameter in the train_test_split function.
