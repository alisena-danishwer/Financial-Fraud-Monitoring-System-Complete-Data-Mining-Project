# Financial-Fraud-Monitoring-System [Complete-Data-Mining-Project]
# 🛡️ Financial Fraud Monitoring System

A data mining project that integrates **multiple techniques** —  
1. Market Basket Analysis  
2. Time Series Forecasting  
3. Recommender Systems  
4. Anomaly Detection  

— to build a robust fraud monitoring and alerting system for financial transactions.  

---

## 🚀 Project Overview
Financial fraud is one of the biggest threats to banking and e-commerce. This project develops a **multi-component fraud monitoring system** that goes beyond traditional anomaly detection by combining association patterns, temporal behavior, recommendation models, and ensemble anomaly detectors.  

**Core idea:**  
- Learn what usually co-occurs in transactions (basket rules).  
- Track when/where/how transactions typically happen (time series).  
- Predict what customers are most likely to purchase (recommender).  
- Flag transactions that deviate from all expectations (anomaly detection).  

---

## 🧩 Components

### 1. Market Basket Analysis
- Uses **Apriori / FP-Growth** to discover frequent item/merchant sets.  
- Identifies unusual combinations of purchases or merchant categories.  

### 2. Time Series
- Forecasts transaction volume/amount per user over time.  
- Models: **ARIMA, Prophet, or LSTM**.  
- Computes **residuals** = actual − expected → used as anomaly features.  

### 3. Recommender System
- Builds **association-rule-based** and **embedding-based (item2vec)** recommenders.  
- Measures the "expectedness" of a purchase for a user.  
- Unlikely merchants/items raise fraud risk.  

### 4. Anomaly Detection
- **Isolation Forest, Autoencoders, One-Class SVM**, and supervised classifiers.  
- Uses ensemble risk scoring.  
- Flags outliers on combined features (association, time, recommender, graph features).  

---

## 📊 Datasets
- **[Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)**  
- Public e-commerce transaction datasets for association-rule mining.  
- (Optional) Synthetic logs for merchant baskets and sequence simulation.  

---

## ⚙️ Tech Stack
- **Python 3.9+**  
- `pandas`, `numpy`, `scikit-learn`, `mlxtend`  
- `statsmodels`, `prophet` (for time series)  
- `gensim` / `surprise` (for recommender)  
- `keras` / `tensorflow` (for autoencoder models)  
- `matplotlib`, `seaborn` (visualization)  
- `Flask` or `Streamlit` (for dashboard deployment)  

## 🏗️ Project Structure


<img width="460" height="614" alt="image" src="https://github.com/user-attachments/assets/0ca06b22-97b7-4f75-8e3f-dd95d53f6088" />



----
## 📌 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/fraud-monitoring-system.git
   cd fraud-monitoring-system

## 📌 Install dependencies:

pip install -r requirements.txt

Run example notebooks (EDA, association rules, time series, recommender, anomaly detection).

Start the dashboard (optional):

bash
streamlit run dashboard/app.py

✅ Evaluation Metrics
Precision, Recall, F1, AUPRC (imbalanced data).

False Positive Rate per 1000 transactions.

Detection lead time (early flagging capability).

📅 Project Timeline
Week 1: Data ingestion & preprocessing

Week 2: Market basket analysis & features

Week 3: Time series modeling & residual features

Week 4: Recommender integration + anomaly detection ensemble

Week 5: Fusion, dashboard, and evaluation

🔮 Future Work
Real-time streaming (Apache Kafka / Spark Structured Streaming).

Graph neural networks for relational fraud detection.

Deployment to cloud (AWS/GCP/Azure) with containerization (Docker).

👨‍💻 Author
Ali Sena Danishwer

Software Developer and Data Scientist

📜 License

This project is licensed under the MIT License - see the LICENSE file for details.



