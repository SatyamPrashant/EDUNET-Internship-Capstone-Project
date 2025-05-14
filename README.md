# Save the README content to a .md file for user to download

readme_content = """
# 💳 Credit Card Default Prediction Using Machine Learning

This project aims to build a classification model to predict whether a customer will default on their credit card payments. Using a dataset of 30,000 records, the system analyzes transactional and demographic data to assist financial institutions in managing credit risk more effectively.

---

## 📂 Dataset

- **Source:** UCI Credit Card Dataset (Taiwan, 2005)
- **Size:** 30,000 rows × 25 columns
- **Target Variable:** `default.payment.next.month` (0 = No Default, 1 = Default)
- **Nature:** Highly imbalanced binary classification problem

---

## 🛠 Preprocessing Steps

1. **Missing Values Handling:**
   - Dataset was clean (no missing or null values)

2. **Feature Engineering:**
   - Added derived features like `total_payment_value` and `dues`

3. **Encoding:**
   - **Label Encoding** for binary/ordinal features (e.g., `SEX`)
   - **One-Hot Encoding** for categorical features (e.g., `EDUCATION`, `MARRIAGE`, `PAY_STATUS` across months)

4. **Class Balancing:**
   - Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance the dataset (original: 78% non-defaulters, 22% defaulters)

5. **Feature Scaling:**
   - Standardized numerical features using `StandardScaler`

---

## 📊 Exploratory Data Analysis (EDA)

- Analyzed relationships between features like `AGE`, `LIMIT_BAL`, `SEX`, `MARRIAGE`, `EDUCATION`, and target variable
- Observed patterns in bill amounts and payment history over 6 months
- Found **recent payment status** and **credit limit** to be strong predictors

---

## 🧠 ML Models Implemented

| Model                | Accuracy | Precision | Recall | F1 Score | AUC-ROC |
|----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression  | 74.96%   | 68.16%    | 78.90% | 73.13%   | 0.75    |
| Random Forest        | 83.43%   | 80.92%    | 85.18% | 82.99%   | 0.84    |
| SVC (RBF Kernel)     | 77.66%   | 71.46%    | 81.56% | 76.18%   | 0.78    |
| XGBoost Classifier   | 82.91%   | 79.43%    | 85.36% | 82.29%   | 0.83    |

---

## 📈 Performance Metrics

- **Accuracy**
- **Precision / Recall / F1-Score**
- **ROC-AUC Score**
- **Confusion Matrix**

---

## ✅ Key Outcomes

- Addressed class imbalance using SMOTE
- Identified high recall models (Random Forest & XGBoost)
- Found credit limit and recent payment status to be most important features

---

## 🔮 Future Scope

- Behavioral pattern analysis to proactively flag high-risk customers
- Build a user-friendly dashboard to input customer info and predict default
- Explore economic impact features such as interest rates or unemployment
- Apply advanced techniques like ensemble learning or deep learning

---

## 🧰 Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn, XGBoost, imbalanced-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📬 Contact

**Satyam Prashant**  
B.Tech AI & DS – IIITDM Kurnool  
📧 satyamprashant2002@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/satyam-prashant/)
"""
