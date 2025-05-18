# 🚀 Titanic ETL Data Pipeline Project

---

## 📌 Project Title:
**ETL Data Pipeline for Titanic Dataset using Pandas and Scikit-learn**

---

## 🎯 Objective / Aim of the Project:

The objective of this project is to develop an **automated ETL (Extract, Transform, Load) pipeline** using Python libraries like **Pandas** and **Scikit-learn**. This pipeline processes raw Titanic dataset (`tested.csv`) by cleaning, transforming, and saving it for further analysis or machine learning tasks.

---

## 🧰 Technologies & Libraries Used:

- **Programming Language:** Python 3.x  
- **Libraries:**
  - `pandas` – for data manipulation
  - `scikit-learn` – for data preprocessing and transformation
  - `joblib` – for saving the pipeline and processed data

---

## 🔄 ETL Process Explanation:

### ✅ 1. Extract
- Load raw data from `tested.csv` using `pandas.read_csv()`.

### ✅ 2. Transform
- Drop unnecessary or sparse columns: `Name`, `Ticket`, `Cabin`, `PassengerId`.
- Handle missing values:
  - `Age`, `Fare` → imputed using mean
  - `Embarked` → imputed using most frequent value
- Encode categorical columns: `Sex`, `Embarked` using One-Hot Encoding.
- Scale numerical features: `Age`, `Fare`, `SibSp`, `Parch`, `Pclass` using `StandardScaler`.

### ✅ 3. Load
- Split the dataset into training and testing sets.
- Save the processed data as `processed_titanic_data.pkl`.
- Save the transformation pipeline as `titanic_pipeline.joblib` for future reuse.

---

## ▶️ How to Run the Project:

### 1. Install required libraries:

```bash
pip install pandas scikit-learn joblib
