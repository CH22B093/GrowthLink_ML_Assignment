# GrowthLink_ML_Assignment
# Credit Card Fraud Detection using XGBoost

##  Project Overview
The main objective of this project is to build a machine learning model that can distinguish fraudulent transactions from legitimate ones.
**XGBoost** model was used.
Reasons:
- **Handles Imbalanced Data well**: Fraudulent detection datasets usually are highly imbalanced. XGBoost can easily integrate with oversampling techniques like **SMOTE**, making it robust against class imbalance.
- **High Predictive Power**: Can capture complex nonlinear patterns and interactions between features, which is common in fraudulent behaviour.

## Objective
- To develop a fraud detection system that **maximizes fraud detection** while **minimizing false positives**.
- To extract meaningful patterns from transactional data and build a reliable classification model.

## Dataset
Training and testing dataset were given separately.The dataset consisted of anonymized transactional data, including features such as:
- Transaction amount
- User ID
- Merchant information
- Timestamp
- Other transaction metadata

The training dataset had 1048575 rows and 23 columns.
Columns like first,last,street etc were disregarded since, they do not contribute to finding the fraudulent behaviour.
> **Note:** The dataset is assumed to be imbalanced, as fraudulent transactions are rare compared to legitimate ones.


## Key Tasks

1. **Data Preprocessing**  
   - Handle missing values and duplicates
   - Encode categorical variables (e.g., merchants, user IDs)
   - Feature engineering (e.g., time-based features, aggregation metrics)
   - Normalize/scale numerical features
   - Address class imbalance using techniques like SMOTE or class weights

2. **Exploratory Data Analysis (EDA)**  
   - Analyze transaction patterns for legitimate vs. fraudulent transactions
   - Visualize key indicators such as transaction amounts, time of day, and merchant behavior

3. **Modeling with XGBoost**  
   - Train/test split and cross-validation
   - Hyperparameter tuning (e.g., using GridSearchCV)
   - Evaluation using metrics like precision, recall, F1-score, ROC-AUC

4. **Model Evaluation**  
   - Focus on reducing false positives while achieving high recall
   - Analyze confusion matrix and feature importance
  
## Expected Outcome
A high performance fraud detection model was obtained.
- The model produced a high recall (97%). Thus, the number of false positives in this model is very low.
- Achieved a ROC-AUC Score of  0.9127560181655932.
- Also, feature importance was studied, i.e which columns contribute to more fraudulent behaviour.

## Tech Stack

- **Python**
- **XGBoost**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib & Seaborn** (for visualization)
- **Imbalanced-learn** (for handling imbalance)

## Results
### Confusion Matrix
  
  ![image](https://github.com/user-attachments/assets/172130b5-f6c3-4bbb-949c-2fdc52718d03)

### Precision-Recall curve
  
  ![image](https://github.com/user-attachments/assets/27643bcb-f287-4093-bc67-04d06e4e777b)

### ROC Curve
  
  ![image](https://github.com/user-attachments/assets/3ec3c4b9-9050-46ca-9041-ad9103cb3a48)

### Feature Importance
  
  ![image](https://github.com/user-attachments/assets/abc2542f-e228-46c5-b528-18e0d6e4a446)

  ### Features:
  
  ![image](https://github.com/user-attachments/assets/601f9572-5457-4def-98bb-aea0907039c2)





