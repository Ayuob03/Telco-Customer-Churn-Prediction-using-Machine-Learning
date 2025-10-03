# Telco Customer Churn Prediction using Machine Learning

## 📌 Overview
This project predicts whether a customer will **churn** using the [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn?utm_source=chatgpt.com).  
The project handles data preprocessing, encoding categorical features, scaling numeric features, handling class imbalance with **SMOTE**, and hyperparameter tuning.  
The main evaluation metric is **F1-score** to account for the imbalanced dataset.

## 📊 Dataset
- **Source:** Kaggle – Telco Customer Churn  
- **Samples:** ~7000 customers  
- **Features:** Customer demographics, account info, service usage (e.g., tenure, InternetService, Contract, PaymentMethod)  
- **Target:** `Churn` (1 = churned, 0 = not churned)  

## ⚙️ Methods
1. **Data Cleaning & Preprocessing**  
   - Handle missing values and incorrect types  
   - Encode Yes/No features to binary  
   - Merge "No internet service" with "No"  
   - One-Hot Encode multi-category features (`InternetService`, `Contract`, `PaymentMethod`)  
   - Scale numeric features  
2. **Handling Class Imbalance**  
   - Use **SMOTE (Synthetic Minority Oversampling Technique)** to balance the minority class in training data  
3. **Modeling & Hyperparameter Tuning**  
   - Models: Logistic Regression, Random Forest, Gradient Boosting,..etc  
   - Hyperparameters tuned using **RandomizedSearchCV**  
   - Evaluation metric: **F1-score**  


## 🛠️ Technologies
- Python  
- Pandas, NumPy  
- scikit-learn  
- imbalanced-learn (SMOTE)  
- Matplotlib, Seaborn  

## 🚀 Usage
Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/telco-churn-prediction.git
cd telco-churn-prediction
pip install -r requirements.txt
