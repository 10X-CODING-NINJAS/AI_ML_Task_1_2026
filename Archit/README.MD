# Social Media Engagement Predictor

## Project Overview
This project builds  Machine Learning pipeline to predict the performance tier (Low, Medium, High, Viral) of a social media post using only **pre-publish structured metadata.**

## Problem Statement
Marketing teams need to understand the potential of a post *before* it goes live. This project isolates valid predictive features (e.g., post hour, media type, follower count) from post-hoc metrics (e.g., likes, reach) to prevent data leakage and evaluate true predictive power.

## Dataset Description
* **Source:** `Instagram_Analytics.csv`
* **Target Variable:** `performance_bucket_label` (4 perfectly balanced classes)
* **Features Used:** Account Type, Follower Count, Media Type, Content Category, Has Call to Action, Post Hour (Cyclically transformed), Day of Week, Caption Length, Hashtags Count.

## Technologies Used
* **Data Processing:** pandas, numpy, scikit-learn (ColumnTransformer, StandardScaler, OneHotEncoder)
* **Modeling:** Logistic Regression, Random Forest Classifier, HistGradientBoostingClassifier
* **Visualization:** matplotlib, seaborn

## Results & Observations
* **The Data Leakage Test:** The primary finding of this project is that pre-publish metadata alone yields a predictive accuracy of ~25% across all tested algorithms. 
* **Engineering Conclusion:** Because the 4 target classes are perfectly balanced (25% each), an accuracy of 25% mathematically represents random guessing. This proves that without the inclusion of post-hoc engagement metrics (which would introduce severe data leakage), static metadata lacks the inherent signal required to predict virality on this specific dataset. 
* **Model Comparison:** While Gradient Boosting marginally outperformed the others (Macro F1: 0.2498), all models converged on the same predictive ceiling.

## Steps to Run the Project
1. Clone this repository.
2. Install dependencies: `pip install pandas numpy scikit-learn matplotlib seaborn`
3. Run the notebooks.