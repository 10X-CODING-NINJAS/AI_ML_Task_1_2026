# INTROVERT-EXTROVERT-AMBIVERT_PREDICTOR

## Project Overview:-
This project builds a Machine Learning predicting model to classify users into Introvert, Extrovert, or Ambivert  based on behavioral and lifestyle feautres. The project follows  EDA, Feature Engineering, Data Preprocessing, Model Training, and Model Evaluation.

## Problem Statement:-
The objective is to build a Classical Machine Learning pipeline capable of predicting personality-related traits such as Introvert, Extrovert, or similar behavioural categories using structured behavioural or social interaction data.

## Dataset description:-
The dataset contains synthetic behavioral data with features related to social interaction, confidence, organization, risk-taking, and lifestyle habits.
It's sourced from kaggle.  **Dataset Source:** https://www.kaggle.com/datasets/miadul/introvert-extrovert-and-ambivert-classification

## Target Variable:
 Personality Type = Introvert Extrovert Ambivert

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- GitHub

## Project Structure

```
INTROVERT-EXTROVERT-AMBIVERT_PREDICTOR/
│
├── INTROVER_EXTROVERT_AMBIVERT.ipynb
├── personality_synthetic_dataset.csv
├── README.md
└── .gitignore
```

---

 ## Machine Learning Workflow

- Data Loading
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Preprocessing
- Train-Test Split
- Model Training
- Model Evaluation
- Model Comparison

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest

## Results

| Model | Accuracy |
|--------|----------|
| Logistic Regression | **99.80%** |
| Decision Tree | **98.55%** |
| Random Forest | **99.68%** |

Logistic Regression achieved the highest accuracy and overall performance on the dataset.

## Performance Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix and these are included in the notebook

## Steps to run the project:-

1. download this repository.
2. Open the notebook in Google Colab.
3. Connect to a Python runtime.
4. Upload the dataset "personality_synthetic_dataset.csv" to the Colab working directory.
5. Run all the cells sequentially.

## References

The following resources were used to understand the concepts and complete this project:

- GeeksforGeeks – Exploratory Data Analysis (EDA)  
  https://www.geeksforgeeks.org/data-analysis/what-is-exploratory-data-analysis/

- YouTube – Exploratory Data Analysis Tutorial  
  https://youtu.be/4P4UxXK7WE8

- Coursera – Machine Learning Specialization by Andrew Ng  
  https://www.coursera.org/specializations/machine-learning-introduction

- ChatGPT (OpenAI) – Used for syntax guidance and also for learning.



