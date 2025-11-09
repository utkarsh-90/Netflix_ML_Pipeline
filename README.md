# 🎬 Netflix Content Engagement Prediction - End-to-End ML Pipeline

**Author:** Utkarsh Panchal  
**Platform:** Google Colab + AWS SageMaker  
**Repository Type:** Full-stack ML Pipeline (data → model → insights)  
**Tech Stack:** Python · pandas · NumPy · scikit-learn · XGBoost · AWS SageMaker · boto3 · Matplotlib · Seaborn  

---

## 🧠 Overview

This project builds an **end-to-end machine-learning pipeline** that predicts how users engage with Netflix titles.  
The model analyzes content metadata (genres, ratings, duration, etc.) to forecast:

- ⭐ **User Rating (1–5)** — Regression  
- ❤️ **User Liked / Not Liked (0 / 1)** — Classification  

It demonstrates how streaming platforms can leverage ML to improve **recommendations**, **catalog decisions**, and **user retention**.

---

## 🎯 Business Motivation

Streaming companies like Netflix depend on predicting **viewer engagement** before a title is released.  
Accurate engagement prediction enables teams to:

- Prioritize which content to promote or license  
- Personalize recommendations for users  
- Allocate production budgets strategically  
- Reduce churn through smarter suggestions  

This notebook turns **raw catalog data → actionable engagement insights**.

---

## ⚙️ Technical Architecture

| Phase | Goal | Tools |
|:------|:-----|:------|
| **1️⃣ Data Preparation** | Cleaning, feature engineering, encoding | pandas · NumPy |
| **2️⃣ Model Training** | Regression + Classification (XGBoost) | scikit-learn · XGBoost |
| **3️⃣ Evaluation** | Compute RMSE, R², Accuracy, Precision, Recall, F1 | sklearn.metrics |
| **4️⃣ Visualization** | Genre + prediction analysis | Matplotlib · Seaborn |
| **5️⃣ Deployment (Optional)** | Realtime endpoint hosting | AWS SageMaker |
| **6️⃣ Monitoring** | Latency + drift tracking | AWS CloudWatch |

---

## 🧩 Pipeline Flow

```text
Raw Netflix Data
     ↓
Data Cleaning & Feature Engineering
     ↓
Train/Test Split (80/20)
     ↓
Model Training (XGBoost Regression + Classification)
     ↓
Model Evaluation & Visualization
     ↓
[Optional] AWS SageMaker Deployment
