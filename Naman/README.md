# INTROVERT-EXTROVERT_PREDICTOR

## Project Overview:-
This project builds a Machine Learning predicting model to classify users into Introvert or Extrovert  based on behavioral and lifestyle feautres. The project follows  EDA, Feature Engineering, Data Preprocessing, Model Training, and Model Evaluation.

## Problem Statement:-
The objective is to build a Classical Machine Learning pipeline capable of predicting personality-related traits such as Introvert, Extrovert, or similar behavioural categories using structured behavioural or social interaction data.

## Dataset description:-
The dataset contains synthetic behavioral data with features related to Time_spent_Alone, Stage_fear, Going_outside, Friends_circle_size, Drained_after_socializing.
It's sourced from kaggle.  **Dataset Source:** https://www.kaggle.com/datasets/rakeshkapilavai/extrovert-vs-introvert-behavior-data

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- GitHub

## Project Structure

```
INTROVERT-EXTROVERT_PREDICTOR/
│
├── Personality_Classification.ipynb
├── personality_dataset.csv
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
| Logistic Regression | **92.41%** |
| Decision Tree | **88.10%** |
| Random Forest | **99.31%** |

 Random forest achieved the highest accuracy and overall performance on the dataset.

## Performance Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Steps to run the project:-

1. Clone the repository.
2. Open the project folder in VS Code.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

4. Open `Personality_Classification.ipynb` in VS Code or Jupyter Notebook.
5. Run all the cells from top to bottom.
 
