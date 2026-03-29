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

The dataset is slightly imbalanced, with a higher number of non-diabetic cases. This imbalance can influence model performance and may lead to bias toward the majority class.
<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/de91f51b-286c-4b0c-bfc4-7bfd786e15d6" />

**Insight:**
The dataset is slightly imbalanced, with more non-diabetic cases.

---

###  Visualization 2: Correlation Heatmap

Glucose shows the strongest correlation with diabetes (~0.49), making it the most influential feature. BMI and Age also contribute moderately, indicating their importance in prediction.
<img width="932" height="849" alt="image" src="https://github.com/user-attachments/assets/d968fd26-a0db-4788-856d-b6111f653a5e" />

**Insight:**
Glucose has the strongest correlation with diabetes, followed by BMI and Age.

---

###  Visualization 3: Glucose Distribution

The distribution is slightly right-skewed, indicating that some patients have significantly higher glucose levels, which may increase diabetes risk.
<img width="716" height="569" alt="image" src="https://github.com/user-attachments/assets/1bf11fc3-451f-47ed-ada8-a77901c2a681" />

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
<img width="914" height="319" alt="image" src="https://github.com/user-attachments/assets/73e2b365-c7d7-4910-bec2-5be8c36c1e05" />

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
