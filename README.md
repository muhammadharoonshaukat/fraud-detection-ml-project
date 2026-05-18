# 📊 Machine Learning-Based End-to-End Fraud Detection System
## 🧾 Project Overview

This project builds a complete end-to-end fraud detection system combining data engineering, analytics, and machine learning. It follows a production-style workflow using Databricks Medallion Architecture, MLflow, and Power BI.

The system is designed to:
- Detect fraudulent transactions in large-scale data
- Monitor fraud risk patterns in real time
- Support data-driven business decisions

## 📁 Dataset & Source
-	Source: Fraud Detection Transactions Dataset (https://www.kaggle.com/datasets/samayashar/fraud-detection-transactions-dataset/data)
-	Time Period: January 2023 – December 2023 
-	Purpose: Used for learning and portfolio purpose
## 📁 Project Workflow
  The project follows a three-stage pipeline architecture

  ### ETL Pipelines (Databricks Medallion Architecture)
#### 🥉 Bronze Layer
- Raw transaction data ingestion
- Preserves original dataset for traceability
#### 🥈 Silver Layer
- Data cleaning and preprocessing
- Handling missing values and duplicates
- Basic business rule validation
#### 🥇 Gold Layer
- Final curated dataset (fraud_gold)

⚙️ Automation
Scheduled workflows for pipeline execution
Ensures fresh, reliable, and consistent data
🔹 MLflow (Machine Learning Pipeline)
Models Used
Logistic Regression (baseline model)
XGBoost (advanced model)
Workflow
Load gold dataset
Perform EDA
Feature engineering
Model training with MLflow tracking
Evaluation and comparison
Model registration
Validation Results
Logistic Regression → F1: 0.7157 | AUC: 0.8962
XGBoost → F1: 0.9994 | AUC: 1.0000
🔹 Automated Power BI Dashboard
Purpose
Real-time fraud monitoring
Risk tracking and visualization
Business decision support
Features
Interactive filters
Time-based analysis
Risk segmentation dashboards
