# Credit Card Fraud Detection
![Image] (https://miro.medium.com/v2/resize:fit:1024/0*nDTApwXjrDUH3kqm.png)
## Problem Statement
The project focuses on detecting fraudulent credit card transactions using machine learning models. With financial institutions facing significant challenges from fraud, machine learning provides an efficient way to monitor transactions, reduce manual reviews, and minimize financial losses. This model aims to identify fraudulent transactions based on historical data from over 1,000 cardholders and 800 merchants, spanning 2019–2020.
## Key Features:
- **Fraudulent Transactions:** Detection of transactions made through stolen, altered, or counterfeit credit cards.
- **Imbalanced Data:** The dataset is highly imbalanced with fraudulent transactions accounting for just 0.52% of all data.
- **Transactional Data:** Includes various features like transaction amount (`amt`) and fraud labels (`is_fraud`).
## Data Understanding
The dataset consists of 1.85 million transactions from 1,000 cardholders with 800 merchants. The target variable (`is_fraud`) labels transactions as fraudulent or legitimate. The data is imbalanced, requiring special techniques for model training and evaluation.
## Project Pipeline
- **Data Understanding:** Analyze and preprocess the data to select relevant features.
- **Exploratory Data Analysis (EDA):** Univariate and bivariate analysis, feature transformation, and handling data skewness.
- **Train/Test Split:** Use stratified k-fold cross-validation to ensure balanced representation of fraud cases.
- **Model Building & Hyperparameter Tuning:** Begin with a baseline linear model, progressing to ensemble methods like Random Forest, Decision Tree, and XGBoost. Hyperparameter tuning is employed for optimization.
- **Model Evaluation:** Focus on recall, precision, and F1-score to maximize the identification of fraudulent transactions.
## Model Evaluation & Selection
The **XGBoost model with Hyperparameter Tuning** on SMOTE data was chosen as the final model:
- **Accuracy:** 99.8%
- **Recall:** 90.7%
- **Precision:** 82.3%
- **ROC:** 99.8%
- **Key Metric:** High recall (90.7%) for accurately identifying fraudulent transactions.
## Business Impact & Recommendations
**Cost-Benefit Analysis:**
- Before model deployment: Banks suffered heavy losses from undetected fraud, reimbursing full transaction amounts for fraudulent cases.
- After model deployment: The model helps identify fraudulent transactions for additional verification, reducing the number of false positives and decreasing overall fraud costs. Estimated cost per fraudulent transaction for the secondary verification service is $1.5.
**Key Business Recommendations:**
- **High Transaction Amounts:** Alert customers if spending exceeds typical patterns.
- **Peak Days for Fraud:** Focus on Thursday, Saturday, and Monday when fraud spikes.
- **High-Risk Categories:** Watch for fraud in categories like home, shopping, grocery, health, and transportation.
- **Time of Day:** Fraudulent transactions mostly occur between 10:00 PM and 3:00 AM.
- **Real-time Alerts:** Implement real-time alerts (SMS/Email) to confirm the legitimacy of suspicious transactions.
## Conclusion
This project demonstrates the power of machine learning in preventing fraud and ensuring financial security for credit card holders. By implementing the model, banks can significantly reduce their fraud-related losses and improve customer trust.

  
