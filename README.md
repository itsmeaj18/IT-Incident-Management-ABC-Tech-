# 🚨 IT Incident Management (ABC Tech)

This project focuses on optimizing IT incident management for ABC Tech, a mid-sized IT services company. By leveraging machine learning and data analytics, we aim to streamline operations, enhance ticket handling efficiency, and support data-driven decision-making in IT service workflows.

## 📌 Problem Statement

ABC Tech handles ~25,000 ITSM incident tickets annually. Traditional process improvements have plateaued, and customer satisfaction has declined. This project introduces Machine Learning (ML) techniques to:

1. **Predict High Priority Tickets**  
2. **Forecast Incident Volume by Department/Quarter**  
3. **Auto-Tag Tickets with Correct Priority and Department**  
4. **Identify RFCs & Asset Misconfigurations**

## 🧠 Machine Learning Use Cases

| Use Case | Objective |
|----------|-----------|
| 🎯 High Priority Ticket Prediction | Classify incoming tickets as High (P1/P2) vs Normal (P3/P4) |
| 📈 Incident Volume Forecasting | Predict ticket trends across quarters and departments |
| 🏷️ Ticket Auto-Tagging | Predict `Priority` and `CI_Cat` for routing automation |
| 🧩 RFC & Asset Misconfiguration Prediction | Detect change failures or misconfigured assets early |

## 📊 Dataset Overview

- ~46,000 real-world ITSM incidents (2012–2014)
- Stored in MySQL, imported and processed in Python
- Key fields:  
  - `Incident_ID`, `Priority`, `Impact`, `Urgency`, `CI_Cat`, `CI_Subcat`, `Status`, `Handle_Time_hrs`, `No_of_Reassignments`, `Closure_Code`, etc.
  - Timestamps: `Open_Time`, `Resolved_Time`, `Close_Time`

## 🛠️ Tech Stack

- **Languages:** Python, SQL  
- **Libraries:** pandas, numpy, plotly, matplotlib, scikit-learn, xgboost, imbalanced-learn  
- **ML Techniques:** Classification (LogReg, RF, XGB), SMOTENC Oversampling, Hyperparameter Tuning  
- **Visualization:** Plotly, Matplotlib  
- **Database:** MySQL

## 🧪 Key Steps Performed

- 🔍 Data Extraction from MySQL
- 🧼 Data Cleaning & Type Conversion
- 📊 EDA with categorical & numerical insights
- 🧠 Feature Engineering (Priority Imbalance, CI Category, Closure Patterns)
- 🧪 Classification Models to Predict High Priority Tickets
- 📈 Forecasting & Volume Trend Analysis

## ✅ Key Results & Insights

- Most tickets were low priority (`P4`) — strong **class imbalance** handled with SMOTE.
- Certain departments (CI_Cat like `application`) dominated the ticket volume.
- High-priority prediction achieved strong recall scores using **XGBoost with SMOTENC**.
- Volume forecasting showed consistent patterns across departments each quarter.

## 🌐 Links

- 🔗 [Kaggle](https://www.kaggle.com/)
- 🧠 [XGBoost Documentation](https://xgboost.readthedocs.io/)
- 🐍 [scikit-learn](https://scikit-learn.org/)
- 📘 [LinkedIn – Ajinkya Itale](https://www.linkedin.com/in/ajinkya-itale-b8048721b)

---  


## 🧑‍💻 Author

**Ajinkya Itale**  
_Data Science & Machine Learning Enthusiast_  
📧 [ajinkyaitale18@gmail.com]  
🔗 [LinkedIn](https://www.linkedin.com/in/ajinkya-itale-b8048721b)


