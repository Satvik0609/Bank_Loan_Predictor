# 🧠 Bank Loan Approval Prediction using Logistic Regression

## 📌 Project Overview
Banks receive thousands of loan applications every day. To minimize financial risk and improve efficiency, they use predictive analytics to decide whether to approve or reject a loan application.

This project uses **Logistic Regression**, a fundamental binary classification algorithm, to predict whether a loan will be **approved (1)** or **not approved (0)** based on the applicant’s financial and demographic information.

---

## 🎯 Objective
Build a predictive model that classifies loan applications into:
- **1 → Approved**
- **0 → Not Approved**

Based on factors such as:
- Applicant Income  
- Co-applicant Income  
- Loan Amount  
- Credit History  
- Loan Term  
- Gender, Education, Marital Status, etc.

---

## 📊 Dataset
**Source:** [Loan Prediction Dataset – Kaggle](https://www.kaggle.com/datasets/ninzaami/loan-predication)

**File Used:** `train_u6lujuX_CVtuZ9i.csv`

**Target Variable:** `Loan_Status` (Y/N → encoded as 1/0)

---

## 🧩 Technologies Used
- **Python 3**
- **Google Colab / Jupyter Notebook**
- **Pandas**, **NumPy** – Data manipulation  
- **Scikit-learn** – Model training & evaluation  
- **Matplotlib** – Visualization  

---

## ⚙️ Project Workflow

### 1️⃣ Data Loading & Exploration
- Loaded dataset using Pandas  
- Checked missing values and data types  
- Encoded target variable (Y/N → 1/0)

### 2️⃣ Data Preprocessing
- Imputed missing values (median for numeric, most frequent for categorical)
- Standardized numerical columns
- One-Hot Encoded categorical columns using `ColumnTransformer`

### 3️⃣ Model Building
- Used **Logistic Regression** with `max_iter=1000`
- Created a complete ML pipeline with preprocessing + model

### 4️⃣ Model Evaluation
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**
- **Confusion Matrix**
- **ROC Curve**

---

## 📈 Results

| Metric | Score |
|--------|-------|
| **Accuracy** | ~82% |
| **Precision** | ~84% |
| **Recall** | ~78% |
| **F1-score** | ~81% |
| **ROC AUC** | ~0.86 |

> *(Your actual scores may vary slightly based on data splits.)*

**Interpretation:**
- The model correctly predicts loan approval status ~82% of the time.  
- High precision and recall show balanced performance.  
- ROC AUC of 0.86 indicates strong class separation capability.  

---

## 🔍 Insights from Logistic Regression
- Applicants with **good credit history** have a much higher chance of loan approval.
- **Higher income** and **lower loan amount** positively influence approval.
- **Bad credit history** and **large loan amounts** reduce approval chances.

---

## 💾 Files in Repository
| File | Description |
|------|--------------|
| `Bank_Loan_Approval_Prediction.ipynb` | Main Colab notebook with code, training & results |
| `train_u6lujuX_CVtuZ9i.csv` | Kaggle dataset used for model training |
| `loan_logreg_pipeline.joblib` | Saved trained model |
| `README.md` | Project documentation (this file) |

---

## 🚀 How to Run the Project

1. **Clone this repo:**
   ```bash
   git clone https://github.com/<your-username>/Bank-Loan-Approval-Prediction.git
   cd Bank-Loan-Approval-Prediction
