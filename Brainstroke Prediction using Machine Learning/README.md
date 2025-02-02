# Brain Stroke Prediction

📌  **Project Overview**

This project aims to predict the likelihood of a person suffering from a stroke based on various health and demographic factors. The dataset used contains information such as age, gender, hypertension, heart disease, BMI, smoking habits, and more. The goal is to build a machine learning model that can accurately classify individuals as stroke or non-stroke cases.

📊 **Dataset**  
- **Source**: [Kaggle - Stroke Prediction Dataset](https://www.kaggle.com/datasets/zzettrkalpakbal/full-filled-brain-stroke-dataset)
- **Size**: 5110 records, 12 features  
- **Features**:
  - gender (Male, Female, Other)
  - age
  - hypertension (0 = No, 1 = Yes)
  - heart_disease (0 = No, 1 = Yes)
  - ever_married (Yes/No)
  - work_type (Private, Self-employed, Govt job, etc.)
  - Residence_type (Urban/Rural)
  - avg_glucose_level
  - bmi
  - smoking_status (formerly smoked, never smoked, smokes, unknown)
  - stroke (0 = No, 1 = Yes) (Target Variable)


🛠️ **Methodology**

**Data Preprocessing**:
- Handling missing values in BMI (replacing with mean).
- Encoding categorical variables using Label Encoding and One-Hot Encoding.
- Feature Scaling using StandardScaler for numerical features.
- Handling class imbalance using SMOTE (Synthetic Minority Oversampling Technique).


**Model Training & Evaluation**:
- **Baseline Model**: Logistic Regression.
- **Other Models Tested**: Decision Tree, Random Forest, XGBoost.
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, Confusion Matrix.



---

**Installation Instructions**:
1. Clone this repository:
  
   git clone https://github.com/88Rehaan88/Machine-learning.git
