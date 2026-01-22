🛡️ UPI Fraud Detection Using Machine Learning
📌 Project Overview

With the rapid adoption of UPI and digital payment systems, detecting fraudulent transactions has become increasingly important. This project demonstrates an end-to-end machine learning pipeline to identify fraudulent UPI transactions using transaction, device, and time-based features.

The solution focuses on building a reliable and interpretable fraud detection model, with Logistic Regression finalized as the production model, and provides a deployable Streamlit-based web application.

🎯 Key Highlights

End-to-end ML pipeline from data generation to deployment

Synthetic UPI transaction dataset with realistic fraud patterns

Comprehensive EDA and correlation analysis

Multiple models evaluated, Logistic Regression finalized

Streamlit web application for real-time fraud prediction

📂 Dataset Description

The dataset is synthetically generated to simulate real UPI transactions.

Features:

transaction_id

timestamp

user_id

receiver_id

amount

transaction_type

location

device_type

is_rooted_device

network_type

time_of_day

is_fraud (target variable)

🔧 Project Workflow

Data Generation

Python-based synthetic data generation

Rule-based and random fraud injection

Data Preprocessing

Timestamp conversion to datetime

Handling categorical and numerical features

No missing values detected

Feature Engineering

Time-based feature extraction (day, month, time of day)

Exploratory Data Analysis (EDA)

Fraud distribution analysis

Transaction and device pattern analysis

Correlation Analysis

Identified weak linear correlations

Justified use of machine learning models

Encoding & Scaling

Label Encoding for categorical variables

Standard Scaling for numerical features

Model Development

Logistic Regression (final model)

Decision Tree

Random Forest

K-Nearest Neighbors

Model Evaluation

Accuracy, Precision, Recall, F1-score

Confusion Matrix analysis

Deployment

Model saved as .pkl with preprocessing artifacts

Streamlit web application for predictions

✅ Final Model Selection

Logistic Regression was finalized due to:

Stable and consistent performance

Interpretability

Suitability for imbalanced datasets using class weights

Ease of deployment

🚀 Streamlit Application

The Streamlit app allows users to:

Enter transaction details

Get fraud probability

View fraud / non-fraud result with visual indicators

⚠️ Limitations

Dataset is synthetic

Limited behavioral and historical features

No real-time data integration

🔮 Future Enhancements

Hyperparameter and threshold tuning

Advanced ensemble models

Real-time data integration

Model explainability (SHAP, feature importance)

🧑‍💻 Technologies Used

Python

Pandas, NumPy

Scikit-learn

Streamlit

📌 Conclusion

This project demonstrates how machine learning can be effectively applied to detect fraudulent UPI transactions. By focusing on a clean pipeline and interpretable models, it provides a strong foundation for real-world fraud detection systems.
