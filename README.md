
# Email Spam Classifier

This project implements an AI/ML solution to classify emails as either SPAM or NOT SPAM (Ham). Using a dataset containing email features and counts of 3000 common words, we train a Multinomial Naive Bayes model, which is well-suited for this type of count-based text data. The project also demonstrates how to deploy the trained model with a Streamlit web interface for real-time predictions.


## Overview

In this project:

- Load a dataset (emails.csv) with 5172 email examples and 3000 features representing word counts.

- Preprocess the data and create a train-test split.

- Train a Multinomial Naive Bayes classifier to predict whether an email is spam.

- Create a CountVectorizer for transforming new email text.

- Save the model and vectorizer.

- Deploy a simple Streamlit web application for real-time spam detection.


## Dataset

The emails.csv file has:

- 5172 rows (emails)

- 3002 columns: the first column is an email identifier, the next 3000 columns are counts of the 3000 most common words, and the final column is the label (1 for spam, 0 for not spam).

- Ensure your dataset is available and update the dataset location in the code accordingly.
## Workflow

#### 1️⃣ Data Loading and Exploration: 
Load and inspect the dataset.

#### 2️⃣ Data Preprocessing and Feature Extraction
Extract features (word counts) and labels from the dataset.

#### 3️⃣ Train-Test Split
Split the data into training and testing sets (e.g., 80/20).

#### 4️⃣ Model Training
Train a Multinomial Naive Bayes model using the training data.

#### 5️⃣ Model Evaluation
Evaluate model performance on the test set.

#### 6️⃣ New Email Prediction
Create a function to transform and predict on new email text.

#### 7️⃣ Model Persistence
Save the trained model and CountVectorizer for future use.

#### 8️⃣ Deployment via Streamlit
Build a web app using Streamlit that allows users to enter email text and see prediction results.
