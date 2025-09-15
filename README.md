# 📊 SyriaTel Customer Churn Prediction  

## 📌 Project Overview  
Customer churn is a critical challenge in the telecom industry, leading to significant revenue losses. This project applies **machine learning models** to predict churn for **SyriaTel** customers, identify the key drivers of churn, and provide actionable recommendations to reduce customer attrition.  

---

## 🎯 Objectives  
- Predict whether a customer will churn (Yes/No).  
- Compare multiple machine learning models for churn prediction.  
- Identify the most important features influencing churn.  
- Provide data-driven recommendations for customer retention.  

---

## 📂 Dataset  
- **Source:** SyriaTel churn dataset  
- **Records:** 3,333 customers  
- **Target:** `churn` (True/False)  
- **Features:**  
  - Demographics: `state`, `area code`, `account length`, `phone number`  
  - Plans: `international plan`, `voice mail plan`, `number vmail messages`  
  - Usage & charges: `total day/eve/night/intl minutes`, `calls`, `charge`  
  - Customer service: `customer service calls`  

---

## 🛠️ Methodology  
The project follows the **CRISP-DM** framework:  
1. **Business Understanding** – Why churn prediction matters.  
2. **Data Understanding** – Exploring class balance and feature distributions.  
3. **Data Preparation** – Encoding, scaling, and resampling with SMOTE.  
4. **Modeling** – Logistic Regression, Decision Tree, Random Forest, XGBoost.  
5. **Evaluation** – Comparing performance using multiple metrics.  
6. **Deployment Recommendation** – Selecting the best model for production.  

---

## 🤖 Model Performance  

| Model                | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression  | 0.86     | 0.83      | 0.86   | 0.84     | 0.60    |
| Decision Tree        | 0.90     | 0.90      | 0.90   | 0.90     | 0.60    |
| Random Forest        | 0.94     | 0.94      | 0.94   | 0.94     | 0.60    |
| **XGBoost**          | **0.94** | **0.94**  | **0.94**| **0.94** | **0.60** |

✅ **XGBoost and Random Forest** gave the strongest overall performance.  

---

## 🔑 Feature Importance  
- **High impact features:**  
  - Customer service calls (frequent calls indicate dissatisfaction).  
  - International plan (customers with this plan are more likely to churn).  
  - Daytime minutes/charges.  
- **Low impact features:**  
  - Account length, area code, phone number.  

---

## 💡 Recommendations  
1. **Prioritize High-Risk Customers** – Focus on customers with high churn probability, frequent service calls, or international plans.  
2. **Improve Customer Service** – Train agents, analyze call logs, and automate common queries.  
3. **Introduce Loyalty Bundles** – Offer bundled international and voicemail plans or heavy-use discounts.  
4. **Maintain the Model** – Retrain quarterly and monitor for performance drift.  
5. **Business Integration** – Deploy the model into the CRM to flag at-risk customers and automate retention workflows.  

---

## 🚀 Deployment Recommendation  
- **XGBoost** is recommended as the production model for its superior balance of accuracy, precision, and recall.  
- **Random Forest** serves as a strong alternative model.  
- **Logistic Regression** remains useful as a baseline.  

---

## 📎 Repository Structure  
x
