# Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview
This project implements a **Credit Card Fraud Detection system** using **supervised machine learning**.  
The goal is to classify credit card transactions as **fraudulent** or **legitimate** based on historical transaction data.

The model is designed as a **backend prediction system**, similar to real-world banking fraud detection pipelines, where transactions are processed automatically rather than through direct user input.

---

## 🧠 Machine Learning Model
- **Algorithm Used:** XGBoost Classifier
- **Learning Type:** Supervised Learning
- **Problem Type:** Binary Classification
  - `0` → Legitimate Transaction  
  - `1` → Fraudulent Transaction

### Why XGBoost?
- Handles **imbalanced datasets** effectively
- Captures **non-linear relationships**
- Provides **high accuracy and robustness**
- Widely used in industry-level fraud detection systems

---

## 📊 Dataset Description

### Dataset Name
**Credit Card Fraud Detection Dataset**

### Source
Kaggle:  
https://www.kaggle.com/mlg-ulb/creditcardfraud

### Dataset Characteristics
- Contains European cardholder transactions
- Highly **imbalanced dataset** (fraud cases are very rare)
- Sensitive features are anonymized using **PCA**

### Feature Explanation
| Feature | Description |
|------|------------|
| Time | Time elapsed (seconds) since first transaction |
| V1 – V28 | PCA-transformed, anonymized features |
| Amount | Transaction amount |
| Class | Target variable (0 = Legitimate, 1 = Fraud) |

⚠️ **Important Note:**  
The PCA features (`V1`–`V28`) do not have human-readable meanings. They are mathematical transformations applied to protect user privacy.

---

## 🚫 Why the Dataset Is Not Included
The dataset file (`creditcard.csv`) is **larger than 100 MB**, which exceeds GitHub’s file size limit.

Therefore:
- The dataset is **excluded using `.gitignore`**
- Users must **download it manually** from Kaggle
- This follows **industry best practices**

---

## ⚙️ How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/ShikhajSomani/Credit-Card-Fraud-Detection-ML-Model.git
cd Credit-Card-Fraud-Detection-ML-Model
