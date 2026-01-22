# UPI Fraud Detection Using Machine Learning

## Project Overview
With the rapid adoption of UPI and digital payment systems, detecting fraudulent transactions has become increasingly important. This project demonstrates an end-to-end machine learning pipeline to identify fraudulent UPI transactions using transaction, device, and time-based features.  
Logistic Regression is finalized as the production model due to its stable and interpretable performance.

## Key Highlights
- End-to-end ML pipeline from data generation to deployment  
- Synthetic UPI transaction dataset with realistic fraud patterns  
- Comprehensive EDA and correlation analysis  
- Multiple models evaluated, Logistic Regression finalized  
- Streamlit web application for real-time fraud prediction  

## Dataset Description
The dataset is synthetically generated to simulate real UPI transactions.

### Features
- transaction_id  
- timestamp  
- user_id  
- receiver_id  
- amount  
- transaction_type  
- location  
- device_type  
- is_rooted_device  
- network_type  
- time_of_day  
- is_fraud (target variable)  

## Project Workflow

### Data Generation
- Python-based synthetic data generation  
- Rule-based and random fraud injection  

### Data Preprocessing
- Timestamp conversion to datetime  
- No missing values detected  
- Data consistency checks  

### Feature Engineering
- Extraction of time-based features (day, month, time of day)  

### Exploratory Data Analysis (EDA)
- Fraud vs non-fraud distribution  
- Transaction type and device analysis  
- Time-based fraud patterns  

### Correlation Analysis
- Correlation heatmap analysis  
- Weak linear relationships observed  
- Justification for machine learning models  

### Encoding and Scaling
- Label Encoding for categorical features  
- Standard Scaling for numerical features  

## Model Development
The following models were developed and evaluated using the same preprocessing pipeline:
- Logistic Regression (final model)  
- Decision Tree  
- Random Forest  
- K-Nearest Neighbors (KNN)  

## Model Evaluation
Models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  

## Final Model Selection
Logistic Regression was finalized due to:
- Balanced and stable performance  
- Interpretability of results  
- Effective handling of class imbalance  
- Ease of deployment  

## Streamlit Application
A Streamlit web application was built to:
- Accept transaction inputs  
- Predict fraud probability  
- Display fraud or non-fraud results visually  

## Limitations
- Dataset is synthetic  
- Limited behavioral and historical features  
- No real-time data integration  

## Future Enhancements
- Hyperparameter tuning  
- Threshold optimization  
- Advanced ensemble models  
- Real-time transaction integration  
- Model explainability (SHAP, feature importance)  

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Streamlit  

## Conclusion
This project demonstrates how machine learning can be effectively applied to detect fraudulent UPI transactions. By focusing on a clean pipeline and interpretable models, it provides a strong foundation for scalable and real-world fraud detection systems.
