# Email Spam Detection using Machine Learning

## Project Overview

This project focuses on developing an email spam detection system using machine learning. The primary goal is to automatically classify incoming emails as "Spam" or "Ham" (not spam). This task was completed as part of the Data Science Internship at Oasis Infobyte under AICTE.

## Features

*   **Data Preprocessing**: Cleaning and preparing email text data.
*   **Feature Engineering**: Converting raw text into numerical features suitable for machine learning.
*   **Machine Learning Model**: Implementation of a Multinomial Naive Bayes classifier for text classification.
*   **Model Evaluation**: Comprehensive assessment of model performance using metrics like accuracy, precision, recall, F1-score, and a confusion matrix.
*   **Custom Testing**: Ability to test the model's predictions on new, unseen email messages.
*   **Simple Rule-Based Detector**: An initial basic Python script to demonstrate the fundamental concept of spam filtering.

## Dataset

The project utilizes the `spam.csv` dataset, which contains real email and SMS messages labeled as either "spam" or "ham." The dataset is preprocessed to create numerical labels for model training.

## Methodology

The core of the project involves a machine learning pipeline within a Jupyter Notebook:

1.  **Data Loading and Cleaning**: Importing `spam.csv` and standardizing column names.
2.  **Label Encoding**: Converting `ham`/`spam` labels to `0`/`1`.
3.  **Data Splitting**: Dividing the dataset into training and testing sets.
4.  **Text Vectorization**: Using `CountVectorizer` to transform text messages into numerical feature vectors.
5.  **Model Training**: Training a `Multinomial Naive Bayes` classifier.
6.  **Model Evaluation**: Generating performance metrics and visualizing the confusion matrix.
7.  **Custom Message Prediction**: Demonstrating the model's ability to classify new messages.

## Results

The machine learning model achieved strong performance, with an accuracy of approximately 97-98%. Key evaluation metrics (precision, recall, F1-score) also indicated robust classification capabilities for both spam and ham messages, with minimal false positives or false negatives. The model accurately identified various custom test messages.

## Project Structure

*   `spam.csv`: The dataset used for training and evaluation.
*   `Task04.ipynb`: Jupyter Notebook containing the full machine learning pipeline.
*   `email_spam_detector.pdf`: A pdf containg project insights
*   `README.md`: This project documentation.

## Setup and Installation

To set up and run this project:

1.  Ensure Python is installed.
2.  Install required libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `jupyter`.
3.  Download `spam.csv` and place it in the project root.
4.  Launch `jupyter notebook` and open `Task04.ipynb` to run the ML model and python code 

## Tools and Libraries Used

*   Python
*   Jupyter Notebook
*   Pandas
*   NumPy
*   Scikit-learn
*   Matplotlib
*   Seaborn

## Conclusion

This project successfully developed an effective spam detection system using machine learning, demonstrating the power of NLP and probabilistic models like Multinomial Naive Bayes to enhance email communication security and efficiency.