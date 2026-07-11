# Extrovert vs Introvert Personality Classification

## Project Overview

This project aims to classify individuals as **Introverts** or **Extroverts** based on their behavioral characteristics using machine learning techniques. Three classification models were trained and compared.

---

## Problem Statement

The objective of this project is to build a machine learning model that can accurately predict whether a person is an Introvert or an Extrovert based on various behavioral features. The project also compares the performance of multiple machine learning algorithms and analyzes the importance of different features in making predictions.

---

### Dataset Features

- Time_spent_Alone
- Stage_fear
- Social_event_attendance
- Going_outside
- Drained_after_socializing
- Friends_circle_size
- Post_frequency

### Target Variable

- Personality
  - Introvert
  - Extrovert

### Data Preprocessing

The following preprocessing steps were performed:

- Removed rows containing missing values in boolean features.
- Replaced missing numerical values using the median.
- Converted Yes/No values into Boolean values (True/False).
- Encoded the target variable using Label Encoding.
- Split the dataset into training and testing sets.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

---

## Machine Learning Models Used

The following classification models were trained:

- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)

Hyperparameter tuning was performed using GridSearchCV.

---

## Results & Observations

- Logistic Regression, Random Forest, and SVM achieved very similar performance after hyperparameter tuning.
- Random Forest was used to analyze feature importance.
- The most influential features were:
  1. Stage_fear
  2. Drained_after_socializing
  3. Time_spent_Alone
  4. Social_event_attendance
- Friends_circle_size contributed the least towards predicting personality.
- The similar performance of all three models suggests that the dataset contains highly informative features, allowing different algorithms to learn similar decision boundaries.

---
