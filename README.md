# Diabetes Prediction Model

##  Project Overview

This project focuses on building a machine learning model to predict whether a person has diabetes based on medical attributes such as glucose level, BMI, and age.

The goal is to demonstrate data preprocessing, exploratory data analysis, and predictive modeling using Python.

---

##  Dataset

The dataset used is the Pima Indians Diabetes Dataset.
Dataset Link : https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

###  Why this dataset?

This dataset is widely used for healthcare prediction tasks and contains relevant medical features. It is suitable for building a classification model and aligns with real-world healthcare applications.

---

##  Data Preprocessing

* Checked for missing values
* Identified invalid zero values in columns like Glucose, BMI, and BloodPressure
* Replaced these values with the mean of respective columns

This step ensures better data quality and improves model performance.

---

##  Exploratory Data Analysis

###  Visualization 1: Class Distribution

A count plot was used to understand the distribution of diabetic and non-diabetic cases.

**Insight:**
The dataset is slightly imbalanced, with more non-diabetic cases.

---

###  Visualization 2: Correlation Heatmap

A heatmap was used to analyze relationships between features.

**Insight:**
Glucose has the strongest correlation with diabetes, followed by BMI and Age.

---

###  Visualization 3: Glucose Distribution

A histogram was used to observe how glucose values are distributed.

**Insight:**
The distribution is slightly skewed, indicating variation in patient glucose levels.

---

##  Model Building

Two machine learning models were used:

* Logistic Regression
* Random Forest Classifier

These models were trained using a train-test split approach.

---

##  Model Output

* Logistic Regression Accuracy: ~76%
* Random Forest Accuracy: ~74–75%

Additional evaluation metrics such as confusion matrix and classification report were used to assess model performance.

---

##  Results & Conclusion

* Glucose was identified as the most important feature influencing diabetes prediction
* Logistic Regression performed slightly better, suggesting linear relationships in the data
* The model provides reliable predictions without overfitting

This solution can be extended to real-world healthcare systems for early diagnosis and better decision-making.

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

##  Files Included

* `task.ipynb` – Jupyter Notebook with complete implementation
* `cleaned_diabetes.csv` – Preprocessed dataset

---
