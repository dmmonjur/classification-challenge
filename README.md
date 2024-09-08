# classification-challenge



## Background

As an Internet Service Provider (ISP), you have been tasked with improving the email filtering system for its customers. To achieve this, you need to develop a supervised machine learning (ML) model that accurately detects spam emails. You have been provided with a dataset containing information about emails, with two possible classifications: spam and not spam. Your goal is to create two classification models—Logistic Regression and Random Forest—to determine which model performs better in detecting spam.

## Files

- **Starter File**: [spam_detector.ipynb](https://github.com/dmmonjur/classification-challenge.git)
- **Dataset**: [Spam Data](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv)

## Before You Begin

1. **Create a Repository**: Create a new repository named `classification-challenge`.
2. **Clone the Repository**: Clone the new repository to your local machine.
3. **Add the Starter File**: Add the starter file `spam_detector.ipynb` to your local repository.
4. **Push Changes**: Push these changes to GitHub or GitLab.

## Instructions

This challenge is divided into the following steps:

### 1. Split the Data into Training and Testing Sets

- **Read the Data**: Load the dataset from [this link](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv) into a Pandas DataFrame.
- **Make a Prediction**: In the appropriate Markdown cell, predict which model you expect to perform better.
- **Create Labels and Features**:
  - Create the labels set (`y`) from the `spam` column.
  - Create the features DataFrame (`X`) from the remaining columns.
- **Check Balance**: Use the `value_counts` function to check the balance of the labels variable (`y`).
- **Split the Data**: Use `train_test_split` to divide the data into training and testing datasets.

### 2. Scale the Features

- **Create an Instance of `StandardScaler`**.
- **Fit the Scaler**: Fit the Standard Scaler with the training data.
- **Scale the Features**: Use the `transform` function to scale both the training and testing features DataFrames.

### 3. Create a Logistic Regression Model

- **Fit the Model**: Train a Logistic Regression model using the scaled training data (`X_train_scaled` and `y_train`) with `random_state` set to 1.
- **Make Predictions**: Use the fitted model to make predictions on the testing data (`X_test_scaled`).
- **Evaluate the Model**: Calculate the accuracy score of the Logistic Regression model using `accuracy_score`.

### 4. Create a Random Forest Model

- **Fit the Model**: Train a Random Forest Classifier model using the scaled training data (`X_train_scaled` and `y_train`) with `random_state` set to 1.
- **Make Predictions**: Use the fitted model to make predictions on the testing data (`X_test_scaled`).
- **Evaluate the Model**: Calculate the accuracy score of the Random Forest Classifier model using `accuracy_score`.

### 5. Evaluate the Models

- **Which Model Performed Better?**: Compare the performance of the Logistic Regression and Random Forest models.
- **How Does That Compare to Your Prediction?**: Reflect on whether your prediction about which model would perform better was accurate and why.

## Requirements

To receive full points for this challenge, ensure your Jupyter notebook includes:

- **Split the Data**:
  - Prediction about which model is expected to perform better.
  - Creation of the labels set (`y`) and features DataFrame (`X`).
  - Balance check of the labels variable using `value_counts`.
  - Data split into training and testing datasets using `train_test_split`.

- **Scale the Features**:
  - Creation and fitting of `StandardScaler`.
  - Scaling of training and testing features.

- **Create a Logistic Regression Model**:
  - Creation and fitting of the Logistic Regression model.
  - Prediction and accuracy evaluation of the model.

- **Create a Random Forest Model**:
  - Creation and fitting of the Random Forest Classifier model.
  - Prediction and accuracy evaluation of the model.

- **Evaluate the Models**:
  - Accurate answers to which model performed better and how it compares to your prediction.

## Example Results

- Logistic Regression Accuracy: 91.97%
- Random Forest Classifier Accuracy: 95.77%

