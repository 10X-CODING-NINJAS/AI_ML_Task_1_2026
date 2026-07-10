# 📊 Social Media Engagement Prediction using Machine Learning

> Predicting **Low, Medium, and High** engagement for social media posts using only **pre-publication metadata**.

![Python](https://img.shields.io/badge/Python-3.13-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikitlearn)
![XGBoost](https://img.shields.io/badge/XGBoost-Gradient%20Boosting-green?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

---

## 📖 Overview

Social media creators often want to estimate how well a post will perform **before publishing it**.

This project builds a complete **Machine Learning pipeline** to classify posts into:

- 🟢 Low Engagement
- 🟡 Medium Engagement
- 🔴 High Engagement

using only metadata available **before the post goes live**.

To simulate a realistic prediction scenario, all post-publication metrics such as Likes, Comments, Shares, Views, and Saves were removed to eliminate data leakage.

---

# 🎯 Objectives

- Perform data cleaning and exploratory data analysis.
- Engineer meaningful predictive features.
- Prevent data leakage.
- Compare multiple ML algorithms.
- Evaluate models using appropriate classification metrics.
- Interpret model predictions using feature importance.

---

# 📂 Dataset

**Dataset Used**

Social Media Engagement Dataset (Kaggle)

The dataset contains metadata such as:

- Platform
- Content Type
- Category
- Follower Count
- Influencer Tier
- Hashtag Count
- Content Length
- Sentiment
- Posting Time
- Day of Week
- Engagement Rate

---

# 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

# ⚙️ Machine Learning Workflow

## 1. Data Cleaning

- Checked missing values
- Removed duplicate records
- Verified data quality

---

## 2. Exploratory Data Analysis

Performed visual analysis of

- Engagement Rate Distribution
- Numerical Feature Distribution
- Categorical Feature Distribution
- Correlation Analysis

---

## 3. Target Variable Creation

Converted continuous **Engagement Rate** into three classes:

| Engagement Rate | Class |
|-----------------|-------|
| < 2% | Low |
| 2% – 6% | Medium |
| > 6% | High |

---

## 4. Data Leakage Prevention

The following columns were removed because they are only available **after publishing**:

- Likes
- Comments
- Shares
- Views
- Saves
- Engagement Rate
- Post ID

This ensures the model predicts engagement using only information known before publication.

---

## 5. Feature Engineering

Created additional features including:

- Hashtag Density
- Weekend Indicator
- Time Bucket
- Influencer Tier Encoding

---

## 6. Data Preprocessing

### Numerical Features

- Standard Scaling

### Categorical Features

- One-Hot Encoding

### Ordinal Features

- Influencer Tier Encoding

Implemented using **Scikit-Learn Pipeline** to avoid data leakage.

---

## 7. Models Trained

Three classical machine learning models were compared.

### Logistic Regression

Simple and interpretable baseline.

### Random Forest

Ensemble of decision trees for nonlinear relationships.

### XGBoost

Gradient Boosted Decision Trees for structured tabular data.

---

# 📈 Model Evaluation

Evaluation Metrics

- Accuracy
- Precision (Macro)
- Recall (Macro)
- F1 Score (Macro)
- Confusion Matrix
- Classification Report
- 5-Fold Cross Validation

---

# 🏆 Results

| Model | Accuracy | Macro F1 |
|--------|----------|----------|
| Logistic Regression | **73.3%** | **72.7%** |
| XGBoost | **74.1%** | **72.6%** |
| Random Forest | **72.3%** | **71.1%** |

Although XGBoost achieved the highest accuracy, **Logistic Regression** achieved the best Macro F1-score and demonstrated the strongest generalization during cross-validation.

---

# 🔄 Cross Validation

| Model | Mean Macro F1 |
|--------|---------------|
| Logistic Regression | **0.728** |
| Random Forest | 0.717 |
| XGBoost | 0.717 |

These results confirm that Logistic Regression provides the most balanced performance.

---

# 📊 Feature Importance

The most influential features were:

- Follower Count
- Influencer Tier
- Platform
- Content Length
- Hashtag Density

These findings align with intuitive expectations about factors affecting engagement.

---

# 📌 Key Insights

- Creator influence strongly affects engagement.
- Platform significantly impacts engagement patterns.
- Feature engineering improved predictive capability.
- Medium engagement posts are the hardest to classify due to overlap with Low and High engagement.

---

# 🚀 Future Improvements

- Hyperparameter tuning using GridSearchCV
- NLP-based caption embeddings
- Image feature extraction using Computer Vision
- Larger real-world datasets
- Model stacking and ensemble learning

---

# 📁 Project Structure

```text
.
├── data/
│   └── social_media_engagement_dataset.csv
│
├── task1.ipynb
├── README.md
├── .gitignore
└── requirements.txt
```

---
# ▶️ Installation & Running the Project

## 1. Clone the official repository

```bash
git clone https://github.com/10X-CODING-NINJAS/AI_ML_Task_1_2026.git
```

## 2. Navigate to submission folder

```bash
cd AI_ML_Task_1_2026/Anmol
```

## 3. Create a virtual environment

```bash
python -m venv .venv
```

## 4. Activate the virtual environment

### Windows

```bash
.\.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

## 5. Install the required dependencies

```bash
pip install -r requirements.txt
```

## 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
task1.ipynb
```

and run all cells sequentially.
---

# 📚 Learning Outcomes

This project demonstrates:

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Machine Learning Pipelines
- Model Comparison
- Cross Validation
- Feature Importance Analysis
- Classification Evaluation
- Data Leakage Prevention

---

# 👨‍💻 Author

**Anmol**

AI/ML Mmeber • Coding Ninjas 10X Club

GitHub: https://github.com/Anmol2627

LinkedIn: https://linkedin.com/in/anmol2627

---

## ⭐ If you found this project useful, consider giving it a star!