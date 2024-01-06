# Spam Email Classification with NLP

## Overview

This repository contains an R Notebook for spam email classification using Natural Language Processing (NLP) techniques. The analysis involves loading and exploring the email dataset, data preparation, tokenization, vectorization, model training, evaluation, and interpretation of results.

## Notebook Details

### 1. Load Required Libraries

- **Libraries:** The script loads necessary R libraries for data manipulation, text processing, and modeling, including `tidyverse`, `text2vec`, `caTools`, and `glmnet`.

### 2. Read and Explore Data

- **Data Reading:** The notebook reads a CSV file containing email data and displays the first few rows and structure of the dataset.

### 3. Data Preparation

- **ID Column Addition:** An 'id' column is added to the dataset defined by the number of rows.

- **Train-Test Split:** The dataset is split into training and testing sets using a seed for reproducibility.

### 4. Tokenization and Vectorization

- **Tokenization:** The training data is tokenized using a preprocessor and word tokenizer.

- **Vocabulary Creation:** A vocabulary is created based on the training data.

- **Vectorization:** The training data is vectorized using a document-term matrix (DTM).

### 5. Model Training

- **glmnet Classifier:** A glmnet classifier is trained using cross-validation with the training data.

### 6. Model Evaluation

- **Coefficients and Feature Importance:** Coefficients and feature importance are extracted from the trained model.

### 7. Testing the Model

- **Tokenization and Vectorization for Testing Data:** The testing data is tokenized and vectorized using the existing vocabulary.

- **Prediction:** Predictions are made on the testing data, and labels are assigned based on a threshold.

### 8. Model Evaluation on Test Set

- **Confusion Matrix:** A confusion matrix is created to evaluate the performance of the model on the test set.

## Dataset Information

### Description

The dataset consists of email subjects labeled as spam or ham (non-spam). Each email subject is binary labeled (0 for ham, 1 for spam).

### Analysis Tasks

1. **Data Import:** Import the emails dataset and get familiarized with it.
2. **ID Column Addition:** Add an 'id' column defined by the number of rows.
3. **Data Preparation:** Prepare data for fitting to the model.
4. **Modeling:** Use `cv.glmnet` for modeling with cross-validation.
5. **Interpretation:** Provide interpretation for both train and test results.

## How to Use

To replicate the analysis:

1. Ensure you have R and the required libraries installed.
2. Place the "emails.csv" dataset in the same directory as the notebook.
3. Run the notebook in an R environment, considering any specific package dependencies.

## Author

- **Author:** html_notebook
- **Date:** 11.04.23


