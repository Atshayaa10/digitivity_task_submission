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

<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/de91f51b-286c-4b0c-bfc4-7bfd786e15d6" />

**Insight:**
The dataset is slightly imbalanced, with a higher number of non-diabetic cases. This imbalance can influence model performance and may lead to bias toward the majority class.

---

###  Visualization 2: Correlation Heatmap
A heatmap was used to analyze relationships between features.

<img width="932" height="849" alt="image" src="https://github.com/user-attachments/assets/d968fd26-a0db-4788-856d-b6111f653a5e" />

**Insight:**
Glucose shows the strongest correlation with diabetes (~0.49), making it the most influential feature. BMI and Age also contribute moderately, indicating their importance in prediction.

---

###  Visualization 3: Glucose Distribution
A histogram was used to observe how glucose values are distributed.

<img width="716" height="569" alt="image" src="https://github.com/user-attachments/assets/1bf11fc3-451f-47ed-ada8-a77901c2a681" />

**Insight:**
The distribution is slightly right-skewed, indicating that some patients have significantly higher glucose levels, which may increase diabetes risk.

---

##  Model Building

Two machine learning models were used:

* Logistic Regression
* Random Forest Classifier

These models were trained using a train-test split approach.

---

##  Model Output
The Logistic Regression model achieved an accuracy of approximately 76%, while the Random Forest model achieved around 74–75%. This level of accuracy is considered good for this dataset because it is relatively small, contains real-world medical data, and has slight class imbalance, making perfect prediction difficult. The slightly better performance of Logistic Regression suggests that the relationship between the input features and the target variable is mostly linear.

The confusion matrix [[83, 16], [20, 35]] provides a deeper understanding of model performance. The model correctly identified 83 non-diabetic patients (true negatives) and 35 diabetic patients (true positives). However, it incorrectly classified 16 non-diabetic patients as diabetic (false positives) and missed 20 diabetic patients (false negatives). In a healthcare context, reducing false negatives is especially important, as missing diabetic cases can delay diagnosis and treatment.

The classification report further evaluates the model using precision, recall, and F1-score. For non-diabetic cases (class 0), the model performs well with a precision of 0.81 and recall of 0.84. For diabetic cases (class 1), the precision is 0.69 and recall is 0.64, indicating that the model is slightly less effective at identifying diabetic patients. Overall, the model demonstrates balanced and reliable performance, but improving recall for diabetic cases would enhance its effectiveness in real-world healthcare applications.
<img width="914" height="319" alt="image" src="https://github.com/user-attachments/assets/73e2b365-c7d7-4910-bec2-5be8c36c1e05" />


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
