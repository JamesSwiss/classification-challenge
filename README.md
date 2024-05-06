# classification-challenge
# Email Filtering System Improvement

## Background
If you work at an Internet Service Provider (ISP), you might have been tasked with improving the email filtering system for its customers. This involves developing a machine learning model to detect spam emails accurately. This Readme provides instructions for building and evaluating two classification models: logistic regression and random forest, using a provided dataset.

## Files
Download the necessary files from [Module 13 Challenge files](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv).

## Before You Begin
1. Create a new repository named `classification-challenge`.
2. Clone the repository to your local machine.
3. Add the `spam_detector.ipynb` starter file to your local repository.
4. Push the changes to GitHub or GitLab.

## Instructions
This challenge includes the following subsections:

### Split the Data into Training and Testing Sets
1. Read the data from [spam-data.csv](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv) into a Pandas DataFrame.
2. Make a prediction about which model you expect to perform better.
3. Create labels (y) from the “spam” column and features (X) DataFrame from the remaining columns.
4. Check the balance of the labels variable (y) using the `value_counts` function.
5. Split the data into training and testing datasets using `train_test_split`.

### Scale the Features
1. Create an instance of `StandardScaler`.
2. Fit the `StandardScaler` with the training data.
3. Scale the training and testing features DataFrames using the `transform` function.

### Create a Logistic Regression Model
1. Fit a logistic regression model with the scaled training data.
2. Save the predictions on the testing data labels.
3. Evaluate the model’s performance by calculating the accuracy score.

### Create a Random Forest Model
1. Fit a random forest classifier model with the scaled training data.
2. Save the predictions on the testing data labels.
3. Evaluate the model’s performance by calculating the accuracy score.

### Evaluate the Models
Answer the following questions:
- Which model performed better?
- How does that compare to your prediction?

## Requirements
Ensure your Jupyter notebook file meets the following criteria:
- Split the Data into Training and Testing Sets (30 points)
- There is a prediction about which model you expect to do better. (5 points)
- The labels set (y) is created from the “spam” column. (5 points)
- The features DataFrame (X) is created from the remaining columns. (5 points)
- The value_counts function is used to check the balance of the labels variable (y). (5 points)
- The data is correctly split into training and testing datasets by using train_test_split. (10 points)
- Scale the Features (20 points)
- An instance of StandardScaler is created. (5 points)
- The Standard Scaler instance is fit with the training data. (5 points)
- The training features DataFrame is scaled using the transform function. (5 points)
- The testing features DataFrame is scaled using the transform function. (5 points)
- Create a Logistic Regression Model (20 points)
- A logistic regression model is created with a random_state of 1. (5 points)
- The logistic regression model is fitted to the scaled training data (X_train_scaled and y_train). (5 points)
- Predictions are made for the testing data labels by using the testing feature data (X_test_scaled) and the fitted model, and saved to a variable. (5 points)
- The model’s performance is evaluated by calculating the accuracy score of the model with the accuracy_score function. (5 points)
- Create a Random Forest Model (20 points)
- A random forest model is created with a random_state of 1. (5 points)
- The random forest model is fitted to the scaled training data (X_train_scaled and y_train). (5 points)
- Predictions are made for the testing data labels by using the testing feature data (X_test_scaled) and the fitted model, and saved to a variable. (5 points)
- The model’s performance is evaluated by calculating the accuracy score of the model with the accuracy_score function. (
