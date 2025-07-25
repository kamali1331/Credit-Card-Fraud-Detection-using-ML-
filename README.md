# Credit-Card-Fraud-Detection-using-ML-Power-BI-Dashboard

# 1. Introduction
# With the rise of digital payments, credit card fraud has become a significant challenge for financial institutions. Traditional rule-based systems fail to detect subtle patterns used by fraudsters. This project aims to develop a machine learning-based fraud detection system that can intelligently flag suspicious transactions and help reduce financial loss. We also integrate Power BI to visualize trends and improve decision-making for fraud analysts.

# 📌 2. Project Overview
# This project uses a real-world credit card transactions dataset that includes over 280,000 records with anonymized features. The goal is to build a classification model that can distinguish between genuine and fraudulent transactions with high accuracy and recall, especially since fraudulent cases represent a very small percentage of the data (imbalanced dataset problem).

# The ML output is then visualized using Power BI, allowing analysts to interact with fraud trends, risk indicators, and transaction behavior.

# 💻 3. Programming Language & Tools Used
# Language: Python
# Libraries:
# Pandas, NumPy – for data handling
# Scikit-learn – for ML models and evaluation
# XGBoost, Logistic Regression, Random Forest – models used
# Matplotlib, Plotly – for visualization
# imblearn – for handling class imbalance (SMOTE)
# Power BI:
# Used to create dashboards with fraud trends, KPIs, and filters
# Integrated using CSV exports from the Python model

# credit-card-fraud-detection/
│
# ├── data/
│   #├── raw_data.csv                  # Original dataset
│   ├── cleaned_data.csv              # Cleaned and preprocessed data
│   └── prediction_results.csv        # Model predictions for Power BI
│
# ├── notebooks/
│   ├── eda_visualization.ipynb       # EDA using Plotly/Matplotlib
│   └── fraud_detection_model.ipynb   # Model training and evaluation
│
# ├── powerbi_dashboard/
│   └── fraud_dashboard.pbix          # Power BI report file
│
# ├── images/
│   └── fraud_dashboard.png           # Screenshot of dashboard
│
# ├── models/
│   └── xgboost_model.pkl             # Trained model (pickle format)
│
├── README.md                         # Project overview and instructions
├── requirements.txt                  # Python libraries required



# 🤖 4. About the Model
# We experimented with multiple models:
# Logistic Regression – for baseline performance
# Random Forest – for robust, ensemble-based prediction
# XGBoost – for high accuracy with optimized boosting

# 🧪 6. Training the Model (Workflow)
# Data Preprocessing:
# Remove duplicates
# Scale Amount and Time using StandardScaler
# Drop irrelevant columns (if any)
# Handle Imbalance:
# Apply SMOTE to balance fraud/genuine classes in training data

# Model Training:
# Train models using train_test_split (80:20)
# Evaluate using metrics: Recall, Precision, F1-score, ROC-AUC
# Prediction & Output:
# Predict fraud probability on test set
# Save results with transaction IDs, amounts, and fraud scores

# Power BI Integration:
# Export cleaned + prediction data as .csv
# Load into Power BI for dashboard creation

# ✅ 6. Merits
# 🎯 High Precision & Recall: ML models outperform manual rules
#  📊 Power BI Dashboards: Easy monitoring of fraud trends
# 🔁 Retrainable: Model can improve with more labeled data
# ⚡ Real-time capable: Can be deployed as an API for streaming detection

# ⚠️ 7. Demerits / Limitations
# ❗ False Positives: May block genuine users occasionally
# 🔍 Data Privacy: Needs secure handling of sensitive data
# 💾 Model Drift: Patterns change over time, requiring regular retraining
# ⚖️ Explainability: Advanced models (like XGBoost) are harder to interpret without SHAP

# 🛑 8. Cautions
# Use balanced evaluation metrics (don't trust accuracy alone)
# Keep fraud experts in the loop for false positive/negative feedback
# Ensure GDPR/PCI compliance while handling personal data
# Don't deploy models trained only on historical data without validating on live data

# Screenshots
# ![Credit card Fraud Detection]<img width="1012" height="525" alt="fraud detection" src="https://github.com/user-attachments/assets/5f4e33b1-e1c6-41c3-a19f-4d25684e0c3e" />
# ![Fraud detection]<img width="1012" height="525" alt="fraud detection 2" src="https://github.com/user-attachments/assets/9dcc9f11-b649-4ae7-b191-e6b9ce9b187c" />



# 🏁 9. Conclusion
# This project demonstrates how Machine Learning can revolutionize the fight against credit card fraud when combined with Power BI dashboards. With intelligent prediction models and dynamic visualization tools, businesses can quickly detect suspicious activities, minimize financial loss, and stay ahead of evolving fraud tactics. Future extensions could include deploying the model Add new featues 

# Welocme to Contributors 
# How to Contribute: Fork the repository
# Create your feature branch: git checkout -b my-feature
# Commit your changes: git commit -am 'Add new feature'
# Push to the branch: git push origin my-feature
# Create a new Pull Request

#  Author : D s kamali [https://github.com/kamali1331]
# Contributors : Jahnvi [https://github.com/jahnavi1708]
#               Ankit kumar [https://github.com/kumar-ankit-100]
#               Tanuja [https://github.com/Tanuja-1708]
#               Lakshaya[https://github.com/Lakshya191]
