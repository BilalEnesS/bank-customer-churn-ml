# Bank Customer Churn Prediction Analysis Report

## 📊 Project Summary

- **Dataset**: Bank Customer Churn Prediction (10,000 customers)
- **Objective**: Customer churn prediction
- **Churn Rate**: 20.37% (2,037 customers)

---

## 🔧 Applied Techniques and Methods

### 1. Data Preprocessing
- **Label Encoding** (country, gender)
- **StandardScaler** normalization
- **Stratified train-test split** (80-20)

### 2. Feature Engineering
- **Age groups**: Young, Middle, Mature, Senior
- **Credit score categories**: Poor, Fair, Good, Excellent
- **Balance categories**: Zero, Low, Medium, High, Very High
- **Customer value score**: balance + salary
- **Loyalty score**: tenure + active_member + products_number
- **Risk score**: age + credit_score - active_member

### 3. Model Algorithms
- Logistic Regression
- Decision Tree
- Random Forest
- **Gradient Boosting** ⭐
- AdaBoost
- XGBoost
- SVM
- K-Nearest Neighbors
- Gaussian Naive Bayes

### 4. Model Optimization
- **GridSearchCV** hyperparameter optimization
- **5-fold cross validation**
- Model selection based on ROC-AUC score

### 5. Model Interpretability
- **Feature Importance** analysis
- **SHAP values**
- **Permutation Importance**
- **Partial Dependence Plots**

---

## 📈 Results and Performance

### 🏆 Best Model: Gradient Boosting

| Metric | Value |
|--------|-------|
| **ROC-AUC** | 0.8655 (86.55%) |
| **Accuracy** | 0.8660 (86.60%) |
| **Precision** | 0.7908 (79.08%) |
| **Recall** | 0.4644 (46.44%) |
| **F1-Score** | 0.5851 (58.51%) |

### 📊 Model Comparison

| Rank | Model | ROC-AUC |
|------|-------|---------|
| 1 | **Gradient Boosting** | 0.8672 ⭐ |
| 2 | AdaBoost | 0.8532 |
| 3 | Random Forest | 0.8524 |
| 4 | SVM | 0.8165 |
| 5 | XGBoost | 0.8310 |

---

## 🎯 Most Important Churn Factors

### 1. Age (34.13% importance)
- **50+ years**: 44.6% churn rate ⚠️
- **18-30 years**: 7.5% churn rate ✅

### 2. Number of Products (24.48% importance)
- **4 products**: 40.0% churn rate ⚠️
- **1-2 products**: 19-20% churn rate

### 3. Active Membership (10.58% importance)
- **Inactive**: 26.9% churn rate ⚠️
- **Active**: 14.3% churn rate ✅

### 4. Gender
- **Female**: 25.1% churn rate ⚠️
- **Male**: 16.5% churn rate ✅

### 5. Country
- **Germany**: 32.4% churn rate ⚠️
- **France**: 16.2% churn rate ✅

---

## 💼 Business Recommendations

### 1. High-Risk Customers
- **Special campaigns** for 50+ year customers
- **Activation programs** for inactive members
- **Gender-specific services** for female customers
- **Special strategy** for Germany market

### 2. Model Deployment
- **Real-time** churn scoring
- **Early warning system**
- **Automatic model updates**
- **Performance monitoring**

### 3. Campaign Strategies
- **Age-group specific** customized products
- **Loyalty programs**
- **Proactive customer relations**
- **Targeted marketing**

---

## ✅ Conclusion

The project was successfully completed. The **Gradient Boosting** model achieved a high performance with **86.55% ROC-AUC** score. The most important churn factors were identified as **age, number of products, and active membership status**.

