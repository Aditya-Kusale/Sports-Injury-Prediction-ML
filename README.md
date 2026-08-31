# 🏥 Sports Injury Prediction Using Machine Learning

An end-to-end Machine Learning project that analyzes athlete-related factors to predict injury risk, injury location, and estimated recovery period.

The project demonstrates multiple Machine Learning approaches including binary classification, multiclass classification, and regression.

---

## 📌 Project Overview

Sports injuries can significantly impact athlete performance and team planning. Early identification of injury risk factors can help support preventive strategies and better recovery management.

This project applies Machine Learning techniques to analyze athlete data and perform three predictive tasks:

1. **Injury Risk Prediction** — Predict whether an athlete is at risk of injury.
2. **Injury Location Prediction** — Predict the potential location/type of injury.
3. **Recovery Period Prediction** — Estimate the expected recovery period.

---

## 🎯 Objectives

- Analyze factors associated with sports injuries.
- Perform Exploratory Data Analysis (EDA).
- Build and compare multiple Machine Learning classification models.
- Predict injury risk using athlete-related features.
- Predict injury location using multiclass classification.
- Estimate injury recovery periods using regression.
- Evaluate model performance using appropriate metrics.
- Identify important features contributing to injury prediction.

---

## 📊 Dataset

The dataset contains **1000 athlete records** with various physical, training, and lifestyle-related features.

### Features Used

- Age
- Training Load
- Previous Injuries
- Recovery Time
- Sleep Quality
- Nutrition Score
- Muscle Fatigue
- Joint Flexibility
- Hydration Level
- Playing Surface

### Target Variables

- Injury Risk
- Injury Location
- Recovery Period

---

## 🔄 Machine Learning Workflow

```text
Data Collection / Generation
          │
          ▼
Data Preprocessing
          │
          ▼
Exploratory Data Analysis
          │
          ▼
Feature Engineering
          │
          ▼
Train-Test Split
          │
          ▼
Feature Scaling
          │
          ├───────────────────────┐
          ▼                       ▼
  Injury Risk Prediction    Additional Predictions
          │                       │
          ▼                       ├── Injury Location
   Model Comparison               │
          │                       └── Recovery Period
          ▼
   Model Evaluation
          │
          ▼
 Final Performance Analysis
