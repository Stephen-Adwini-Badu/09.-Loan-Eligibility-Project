# Loan Prediction Project

## Project Objective
This project aims to predict loan eligibility for potential customers based on various financial, demographic, and personal attributes. By employing machine learning models, the notebook explores how well different algorithms can classify loan applicants into eligible or non-eligible categories.

## Dataset Description
Two datasets are used in this project:
- **Training Dataset:** Contains labeled data to train models.
- **Testing Dataset:** Contains unlabeled data for model evaluation.

## Methodology
### 1. Data Exploration and Preprocessing
- **Loading Data:** Importing training and testing datasets.
- **Data Cleaning:** Handling missing values, duplicates, and inconsistent data.
- **Data Transformation:** Encoding categorical variables for machine learning models.

### 2. Exploratory Data Analysis (EDA)
- **Data Insights:** Analyzing distributions, relationships, and summary statistics of features.
- **Visualization Techniques:** Utilizing Seaborn and Matplotlib to identify trends and correlations.

### 3. Feature Engineering
- Selecting relevant features based on data insights.
- Handling categorical data through label encoding and other transformations.
- Normalizing continuous variables where appropriate.

### 4. Model Training and Evaluation
- Splitting the dataset into training and testing subsets.
- Training machine learning models:
  - Random Forest Classifier
  - Gradient Boosting Classifier
  - XGBoost Classifier
- Evaluation metrics include:
  - Accuracy
  - Precision, Recall, F1-Score
  - ROC-AUC Score
  - Confusion Matrix Visualization

## Machine Learning Models
- **Random Forest Classifier:** Ensemble learning method for classification tasks.
- **Gradient Boosting Classifier:** Boosting technique for improved predictive accuracy.
- **XGBoost Classifier:** Extreme Gradient Boosting implementation optimized for speed and performance.

## Results and Metrics
- **Model Performance:** Comparison of accuracy, precision, recall, and ROC-AUC scores across models.
- **Confusion Matrix:** Provides insights into true positives, true negatives, false positives, and false negatives.

![Image](https://github.com/user-attachments/assets/91edd08e-8527-421b-83c1-2cc37932cef1)

## Conclusion and Future Work
- **Key Insights:** Identification of strong predictors for loan eligibility.
- Strong Indicators: **Loan Perccentage of Income**, **Grade D Loan**, **Home Ownership**

![Image](https://github.com/user-attachments/assets/14968823-974b-4819-a090-108abfd93438)
  
- **Potential Improvements:**
  - Incorporate additional data sources for richer features.
  - Explore hyperparameter optimization for model improvement.
  - Deploy the model as a web service for real-time predictions.
