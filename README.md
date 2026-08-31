# 🏥 Sports Injury Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Project Overview

Sports injuries can be influenced by multiple factors such as training load, previous injuries, muscle fatigue, sleep quality, nutrition, hydration, and joint flexibility.

This project uses Machine Learning to predict whether an athlete is at **high risk of injury** based on several physical and lifestyle-related factors.

The project demonstrates a complete Machine Learning workflow including:

* Synthetic dataset generation
* Exploratory Data Analysis (EDA)
* Data preprocessing
* Baseline model evaluation
* Multiple Machine Learning model comparison
* 5-Fold Cross Validation
* Model evaluation using multiple metrics
* Confusion Matrix and ROC Curve visualization
* Feature importance analysis
* Model persistence using Joblib

---

## 🎯 Problem Statement

The objective of this project is to build a Machine Learning classification model capable of predicting:

> **Whether an athlete is at high risk of sustaining a sports injury.**

The prediction is based on physical condition, training intensity, injury history, and lifestyle-related features.

---

## 🤖 Machine Learning Task

This project focuses on:

### Binary Classification

Target Variable:

| Injury Risk | Meaning   |
| ----------- | --------- |
| 0           | Low Risk  |
| 1           | High Risk |

The following Machine Learning algorithms are compared:

* Logistic Regression
* Support Vector Machine (SVM)
* Random Forest Classifier

A Dummy Classifier is also used as a baseline to verify that the trained models perform better than a naive prediction strategy.

---

# 📊 Dataset Features

The dataset is synthetically generated for educational and experimental purposes.

| Feature           | Description                              |
| ----------------- | ---------------------------------------- |
| Age               | Age of the athlete                       |
| Training_Load     | Intensity of training                    |
| Previous_Injuries | Number of previous injuries              |
| Sleep_Quality     | Quality of sleep                         |
| Nutrition_Score   | Overall nutrition quality                |
| Muscle_Fatigue    | Level of muscle fatigue                  |
| Joint_Flexibility | Flexibility level of joints              |
| Hydration_Level   | Hydration condition                      |
| Playing_Surface   | Type of playing surface                  |
| Injury_Risk       | Target variable representing injury risk |

---

# 🔄 Machine Learning Workflow

```text
Synthetic Data Generation
          │
          ▼
Exploratory Data Analysis
          │
          ▼
Data Preprocessing
          │
          ▼
Train-Test Split
          │
          ▼
Dummy Baseline Model
          │
          ▼
Train Multiple ML Models
          │
     ┌────┼────┐
     ▼    ▼    ▼
   LR    SVM   RF
     │    │    │
     └────┼────┘
          ▼
5-Fold Cross Validation
          │
          ▼
Model Comparison
          │
          ▼
Best Model Evaluation
          │
     ┌────┼───────────┐
     ▼    ▼           ▼
Confusion ROC      Feature
Matrix     Curve   Importance
          │
          ▼
Save Best Model
```

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Joblib
* Jupyter Notebook

---

# 📂 Project Structure

```text
Sports-Injury-Prediction-ML/
│
├── README.md
├── requirements.txt
├── .gitignore
├── SPORTSJINJURY.ipynb
│
├── models/
│   └── injury_risk_pipeline.pkl
│
└── preprocessing/
    └── feature_names.pkl
```

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone https://github.com/Aditya-Kusale/Sports-Injury-Prediction-ML.git
```

## 2. Navigate to the Project Directory

```bash
cd Sports-Injury-Prediction-ML
```

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## 4. Run the Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
SPORTSJINJURY.ipynb
```

Then run all cells.

---

# 📊 Exploratory Data Analysis

The dataset is analyzed to understand:

* Dataset structure
* Missing values
* Statistical summary
* Injury risk distribution
* Feature relationships

Visualization techniques are used to identify patterns between athlete characteristics and injury risk.

---

# 🔧 Data Preprocessing

The preprocessing pipeline includes:

* Encoding categorical variables
* Feature selection
* Train-test splitting
* Feature scaling where required

To prevent data leakage, preprocessing steps are included inside Scikit-learn Pipelines.

---

# 📈 Model Evaluation

The models are evaluated using multiple classification metrics:

### Accuracy

Measures the percentage of correctly predicted samples.

### Precision

Measures how many predicted high-risk cases were actually high-risk.

### Recall

Measures how effectively the model identifies actual high-risk athletes.

### F1 Score

Provides a balance between Precision and Recall.

### ROC-AUC Score

Measures the model's ability to distinguish between low-risk and high-risk athletes.

---

# 🔁 Cross Validation

The project uses **5-Fold Stratified Cross Validation**.

This provides a more reliable estimate of model performance compared to relying only on a single train-test split.

---

# 📊 Baseline Model

A Dummy Classifier is used as a baseline model.

The purpose of the baseline is to ensure that the Machine Learning models provide meaningful improvement over a simple naive prediction strategy.

---

# 🔍 Feature Importance

Random Forest is used to analyze feature importance.

This helps identify which factors contribute most significantly to injury risk prediction.

Examples of potentially important features include:

* Previous injuries
* Muscle fatigue
* Training load
* Sleep quality
* Hydration level

---

# 💾 Model Persistence

The best-performing model is saved using Joblib.

```text
models/injury_risk_pipeline.pkl
```

The feature names are also saved:

```text
preprocessing/feature_names.pkl
```

The saved pipeline can later be used for predictions without retraining the model.

---

# ⚠️ Important Limitation

The dataset used in this project is **synthetically generated**.

Therefore:

> High model performance should not be interpreted as real-world clinical or medical predictive performance.

The project is intended for:

* Educational purposes
* Machine Learning experimentation
* Demonstrating an end-to-end ML workflow

Real-world deployment would require validated sports medicine data and domain expert involvement.

---

# 🚀 Future Improvements

Possible future improvements include:

* Using real-world sports injury datasets
* Increasing dataset size
* Hyperparameter optimization
* Additional Machine Learning algorithms
* Explainable AI techniques such as SHAP
* Deep Learning approaches
* Deployment using Streamlit
* Building a web-based prediction interface

---

# 📌 Key Learning Outcomes

This project demonstrates knowledge of:

* Machine Learning classification
* Data preprocessing
* Feature engineering
* Model comparison
* Cross Validation
* Classification metrics
* ROC Curve analysis
* Feature importance
* Scikit-learn Pipelines
* Model serialization

---

# 👨‍💻 Author

**Aditya Kusale**

GitHub: https://github.com/Aditya-Kusale

---

## ⭐ If you found this project useful

Consider giving the repository a star!
