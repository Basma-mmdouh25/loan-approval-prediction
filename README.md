# Loan Approval Prediction

Task 4 at Internship Project at Elovve

## 📌 Description
This project builds a **predictive machine learning model** to determine whether a loan application will be approved.  
Dataset used: **Loan-Approval-Prediction-Dataset** (Kaggle).  

- **Dataset Link:** [Loan-Approval-Prediction-Dataset](https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset)  
- **Notebook on Kaggle:** [Loan Approval Prediction Notebook](https://www.kaggle.com/code/basmammdouh/loan-approval-prediction)

---

## 📊 Project Workflow

### 1️⃣ Data Exploration
- Loaded and examined dataset using:
  - `info()`, `describe()`, `shape`, `columns`, `isna().sum()`
  - Checked and confirmed **no missing values** or **duplicate rows**.
- Detected and handled **outliers** using IQR method.
  - Visualized with **boxplots before and after treatment**.
- Cleaned **column names** and ensured correct **data types**.
- Visualized **numeric feature distributions** with histograms.
- Displayed **categorical feature value counts** using horizontal bar plots.

---

### 2️⃣ Data Preprocessing
- Reconfirmed no missing values.
- Split features into:
  - **Categorical columns** → Encoded using appropriate encoding techniques.
  - **Numerical columns** → Scaled to normalize distributions.
- Prepared dataset for modeling.

---

### 3️⃣ Modeling & Evaluation

#### **Before SMOTE (Original Imbalanced Data)**
- **Logistic Regression**
  - Accuracy: **~87.2%**
- **Decision Tree**
  - Accuracy: **~97%**

#### **After SMOTE (Balanced Data)**
- **Logistic Regression**
  - Accuracy: **~88.3%**
- **Decision Tree**
  - Accuracy: **~97.3%**

---

### 4️⃣ Model Performance Metrics
For each model:
- Calculated:
  - **Precision**
  - **Recall**
  - **F1-score** (main focus for imbalanced classification)
- Generated:
  - **Classification reports**
  - **Confusion matrices**
  - **Confusion matrix plots** for visual analysis.

---

## 🛠 Tools & Libraries
- **Python**
- **Pandas** – Data manipulation
- **Matplotlib / Seaborn** – Visualization
- **Scikit-learn** – Model building & evaluation
- **Imbalanced-learn (SMOTE)** – Handle class imbalance

---

## 📄 Project Summary
This notebook demonstrates a complete machine learning pipeline:
- Exploratory Data Analysis (EDA)
- Data preprocessing (encoding, scaling, outlier handling)
- Model building (Logistic Regression, Decision Tree)
- Evaluation with focus on **imbalanced binary classification**
- SMOTE resampling to improve model performance
