# 🏦 Customer360 AI Platform with BigQuery ML

![BigQuery](https://img.shields.io/badge/BigQuery-ML-blue?logo=googlecloud)
![Hackathon](https://img.shields.io/badge/Hackathon-Build-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Overview
Customer retention, fraud prevention, and personalization are critical challenges for financial institutions.  
This project builds a **Customer360 AI Platform** using **Google BigQuery ML + Generative AI** to unify:
- ✅ Churn Prediction  
- ✅ Fraud Detection  
- ✅ Spend Forecasting  
- ✅ Product Recommendations  
- ✅ Complaint Classification with LLMs  

All components come together into a **single Customer360 dashboard** for bankers and analysts.

---

## 📂 Dataset
We leveraged public datasets (Kaggle & CFPB) to simulate a financial environment:
- **Transactions Fraud Dataset** (Kaggle) – customer transactions with fraud labels  
- **Card Data** – product ownership information  
- **Users Data** – demographics (age, gender, income, location)  
- **MCC Codes** – merchant categories  
- **CFPB Complaints** – real-world consumer complaint text  

---

## ⚙️ Project Workflow

```mermaid
flowchart TD
    A[Users Data] --> C360
    B[Transactions Data] --> C360
    C[Card Data] --> C360
    D[Complaints Data] --> C360
    C360[Customer360 AI Platform] --> F[Banker Dashboard]
    
    C360 -->|Churn| G[Retention Actions]
    C360 -->|Fraud| H[Alerts]
    C360 -->|Forecast| I[Spend Trends]
    C360 -->|Recommender| J[Next-Best Product]
    C360 -->|LLM Insights| K[Complaint Categories]
