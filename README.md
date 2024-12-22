# Sentiment Analysis for Mental Health

This Jupyter Notebook performs sentiment analysis on a dataset of mental health-related statements.  The goal is to classify the sentiment expressed in each statement.
## Dataset

The dataset used in this notebook is available at: [https://www.kaggle.com/datasets/suchintikasarkar/sentiment-analysis-for-mental-health](https://www.kaggle.com/datasets/suchintikasarkar/sentiment-analysis-for-mental-health)

**To download the dataset:**

1. Go to the Kaggle link above.
2. Click on the "Download" button.
3. Save the downloaded file (`samh.csv` or similar) to the same directory as this notebook, or adjust the file path in the notebook accordingly.  The code expects the file to be named `samh.csv`.

## Notebook Overview

1. **Data Loading and Preprocessing:**
   - Imports necessary libraries.
   - Loads the dataset from `samh.csv`.
   - Handles missing values.
   - Cleans the text data using lowercasing, punctuation removal, stop word removal, and lemmatization.

2. **Feature Extraction:**
   - Uses TF-IDF vectorization to convert text data into numerical features.

3. **Model Training:**
   - Splits the data into training and testing sets.
   - Evaluates multiple classification models (Logistic Regression, Random Forest, SVM, and Naive Bayes) using cross-validation and hyperparameter tuning.
   - Identifies the best-performing model based on accuracy.

4. **Model Saving and Loading:**
   - Saves the best-performing model using `joblib`.
   - Demonstrates how to load the saved model.

5. **Prediction on New Data:**
   - Provides an example of how to use the loaded model to make predictions on new, unseen statements.
