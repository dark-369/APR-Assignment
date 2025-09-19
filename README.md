# 🍷 Wine Quality Prediction using Logistic Regression

## 📌 Introduction
This project predicts wine quality based on physicochemical features using **Logistic Regression**.  
Wine quality (0–10) is transformed into a **binary classification problem**:
- **Good Wine (1):** Quality ≥ 7  
- **Not Good Wine (0):** Quality ≤ 6  

The project demonstrates data preprocessing, model building, hyperparameter tuning, and evaluation using scikit-learn.

---

## 📊 Dataset
- **Source:** [UCI Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- **Samples:** Red wine (1599)
- **Features:** 11 physicochemical properties (acidity, sugar, chlorides, alcohol, etc.)  
- **Target:** Binary label (Good vs Not Good wine)  

---

## 🛠️ Methodology
1. Load dataset and preprocess (binary target, scaling).  
2. Train-test split (80–20, stratified).  
3. Build pipeline: StandardScaler + Logistic Regression.  
4. Tune hyperparameters with GridSearchCV.  
5. Evaluate using Accuracy, Precision, Recall, F1.  
6. Interpret results (feature importance).  

---

## ⚙️ Tools & Libraries
- Python, Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

## 📈 Results
- **Accuracy:** ~82%
- **Important Features:**  
  - Positive: Alcohol, Sulphates  
  - Negative: Volatile acidity  

---

## ✅ Conclusion
- Logistic Regression provides an interpretable baseline with good performance.  
- Alcohol and sulphates strongly influence wine quality, while volatile acidity lowers it.  
- Future improvements: SMOTE oversampling, advanced models (Random Forest, XGBoost).  
