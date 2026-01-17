# Fraud-Detection-with-Explainable-AI

## 🔍 Project Overview
This project addresses the challenge of identifying fraudulent credit card transactions within a highly imbalanced dataset (0.17% fraud rate). Beyond simple classification, the system integrates a Model Interpretability Layer using SHAP to explain exactly why a transaction was flagged, transforming a "black-box" model into an actionable business tool.

## 🚀 Key Features
1. Advanced Imbalance Handling: Implemented Cost-Sensitive Learning (XGBoost scale_pos_weight) and SMOTE-Tomek hybrid resampling to address extreme class skew.
2. High-Precision Modeling: Achieved an AUC-PR of 0.873 and an 83% Recall, effectively identifying the majority of fraud while maintaining low false-positive rates.
3. Explainable AI (XAI): Integrated SHAP (SHapley Additive exPlanations) to provide local and global feature importance, allowing for human-in-the-loop verification.
4. Interactive Dashboard: Developed a simulation interface to visualize how specific feature changes (e.g., shifts in V14 or V17) impact the model's risk score.

##🛠️ Tech Stack 
1. Language: Python 3.9+
2. Database: SQL (SQLite) for data preparation and querying
3. ML Libraries: XGBoost, Scikit-Learn, Imbalanced-learn
4. Interpretability: SHAP, LIME
5. Visualization: Seaborn, Matplotlib, TailwindCSS (for Dashboard)

## 📊 Performance Summary
Metric |  Value  |  Interpretation
AUC-PR,0.873,High skill in minority class identification
Recall,83%,Caught 81 out of 98 fraudulent cases
Precision,86%,Only 13 false alarms out of 56k+ transactions
F1-Score,0.84,Robust balance between precision and recall
