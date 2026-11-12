# Spam / Ham SMS Classification

A machine learning application that classifies SMS messages as **Spam** or **Ham (Legitimate)** using Natural Language Processing (NLP) and a Random Forest Classifier. The model processes user-provided messages and predicts whether they are potentially unwanted or legitimate.

## Overview

This project uses machine learning and text-processing techniques to identify spam messages. It transforms raw SMS text into numerical features using TF-IDF vectorization and uses a trained Random Forest model to perform binary classification.

The trained model is integrated into a Streamlit web application, allowing users to enter messages and receive predictions through a simple interface.

## Features

- **Text Preprocessing:** Converts text to lowercase, tokenizes messages, removes punctuation, non-alphanumeric characters and stopwords, and applies stemming using Porter Stemmer.
- **TF-IDF Vectorization:** Converts processed text into numerical representations for machine learning.
- **Random Forest Classification:** Uses an ensemble learning algorithm to distinguish between spam and legitimate messages.
- **Real-time Prediction:** Accepts user input and generates instant classifications.
- **Streamlit Interface:** Provides an interactive web application for testing SMS messages.

## Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Machine Learning | Scikit-learn |
| NLP | NLTK |
| Data Processing | Pandas, NumPy |
| Feature Extraction | TF-IDF Vectorizer |
| Classification | Random Forest Classifier |
| Model Serialization | Pickle |
| Deployment | Streamlit |

## Project Workflow

1. **Data Preparation:** Load and prepare the SMS dataset for binary classification.
2. **Text Preprocessing:** Clean and normalize SMS messages through tokenization, stopword removal, punctuation removal, and stemming.
3. **Feature Extraction:** Apply TF-IDF vectorization to convert text into numerical features.
4. **Model Training:** Train a Random Forest Classifier using the extracted features.
5. **Model Serialization:** Save the trained classifier and TF-IDF vectorizer using Pickle.
6. **Deployment:** Integrate the saved models into a Streamlit application for interactive predictions.

## Model Information

**Algorithm:** Random Forest Classifier

**Feature Extraction:** TF-IDF (Term Frequency–Inverse Document Frequency)

**Classification Type:** Binary Classification

| Label | Classification |
|---|---|
| 0 | Ham |
| 1 | Spam |

Random Forest gained an accuracy of approximately 97% and precision of 98%.
