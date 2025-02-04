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
  - ROC-AUC and Calibration Curves
  - Feature Importance

## Machine Learning Models
- **Random Forest Classifier:** Ensemble learning method for classification tasks.
- **Gradient Boosting Classifier:** Boosting technique for improved predictive accuracy.
- **XGBoost Classifier:** Extreme Gradient Boosting implementation optimized for speed and performance.

## Results and Metrics
- ### Model Performance:
   Overall, while all three models have excellent performance, **X Gradient Boosting** appears to have a **slight edge in terms of recall, F1 score, and ROC-AUC.**

   - **Similar Accuracy:**  
   All three models have the same **high accuracy of 95.0%**, indicating that they are equally good at predicting the correct class.  

   - **XGB has slightly better Recall and F1 score:**  
   X Gradient Boosting has a **slightly higher recall (74.0%)** and **F1 score (81.0%)** compared to the other two models.  

   - **Random Forest has slightly better Precision:**  
   Random Forest has a **slightly higher precision (93.0%)** compared to Gradient Boosting **(92.0%)** and X Gradient Boosting **(90.0%).**  

   - **XGB has slightly better ROC AUC:**  
   X Gradient Boosting has a **slightly higher ROC AUC (86.0%)** compared to the other two models **(85.0%).** <p>

   <table align="center">
     <tr>
       <th>MODEL</th>
       <th>ACCURACY</th>
       <th>PRECISION</th>
       <th>RECALL</th>
       <th>F1 SCORE</th>
       <th>ROC-AUC</th>
     </tr>
     <tr>
       <td>Random Forest Classifier</td>
       <td align="center">95.0%</td>
       <td align="center">93.0%</td>
       <td align="center">71.0%</td>
       <td align="center">80.0%</td>
       <td align="center">85.0%</td>
     </tr>
     <tr>
       <td>Gradient Boosting Classifier</td>
       <td align="center">95.0%</td>
       <td align="center">92.0%</td>
       <td align="center">71.0%</td>
       <td align="center">80.0%</td>
       <td align="center">85.0%</td>
     </tr>
     <tr>
       <td>X Gradient Boosting Classifier</td>
       <td align="center">95.0%</td>
       <td align="center">90.0%</td>
       <td align="center">74.0%</td>
       <td align="center">81.0%</td>
       <td align="center">86.0%</td>
     </tr>
   </table>

 - ### Confusion Matrix
   - **All three models (Random Forest, Gradient Boosting, and XGBoost)** demonstrate **strong accuracy** in identifying true defaulters (85%) and show **low misclassification** rates for defaulters as paid (ranging from 0.8% to 1.1%). 

   - The models also have **low false positive rates** for true payers (around 4%), with the **XGBoost model slightly outperforming** the others in this aspect. Overall, the models are **highly effective and reliable** in distinguishing between defaulters and true payers.

 ![9 1](https://github.com/user-attachments/assets/e6c27ce1-988c-42e4-92c4-54ba71f5451d)

  
 - ### ROC-AUC and Calibration Curves:
   - **All three models (RFC, GBC, XGB)** have **comparable performance** in terms of distinguishing between classes, as indicated by **similar AUC values**. This suggests that **none of the models consistently outperforms the others** in terms of classification accuracy.
   
   - **The calibration curves for all three models** are **close to the perfect** calibration line (red dashed line), indicating that the predicted probabilities are well-calibrated and reflect the true likelihood of the positive class.

 ![9 2](https://github.com/user-attachments/assets/903b78b4-0280-49e5-ae5c-06ca72e4e4bb)

 - ### Feature Importance
   - With regards to feature importance the most consistently influencial feature was **Loan Percentage Income and Grade D Loan**  
   - Other notables features were;  
     - **Loan Interest Rate**  
     - **Rent Type Home Ownership**

 ![Image](https://github.com/user-attachments/assets/14968823-974b-4819-a090-108abfd93438)