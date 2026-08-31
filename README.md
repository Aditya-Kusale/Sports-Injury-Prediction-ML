# 🏥 Sports Injury Prediction Using Machine Learning

An end-to-end Machine Learning project that analyzes athlete-related factors to predict **injury risk**, **injury location**, and **estimated recovery period**.

The project demonstrates multiple Machine Learning approaches, including **binary classification, multiclass classification, and regression**, along with exploratory data analysis and model performance evaluation.

---

## 📌 Project Overview

Sports injuries can significantly affect athlete performance and training continuity. Identifying patterns associated with injury risk can help support preventive strategies and improve understanding of factors related to athlete health and recovery.

This project applies Machine Learning techniques to analyze athlete-related data and perform three predictive tasks:

1. **Injury Risk Prediction** — Predict whether an athlete is at risk of injury.
2. **Injury Location Prediction** — Predict the potential injury location.
3. **Recovery Period Prediction** — Estimate the expected recovery period.

---

## 🎯 Objectives

- Perform Exploratory Data Analysis (EDA).
- Analyze relationships between athlete-related features and injury outcomes.
- Build and compare multiple Machine Learning models.
- Predict injury risk using binary classification.
- Predict injury location using multiclass classification.
- Estimate recovery periods using regression.
- Evaluate models using appropriate performance metrics.
- Identify important features contributing to predictions.

---

## 📊 Dataset

The project uses a dataset containing athlete-related physical, training, and lifestyle factors.

### Features

The dataset includes features such as:

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

The project focuses on three prediction targets:

- **Injury Risk**
- **Injury Location**
- **Recovery Period**

> ⚠️ **Note:** The dataset used in this project is synthetically generated for educational purposes. Therefore, the results should not be interpreted as clinically validated predictions.

---

# 🔄 Machine Learning Workflow

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
Train-Test Split & Feature Scaling
          │
          ▼
┌─────────────────────────────────────┐
│       Machine Learning Models       │
├─────────────────────────────────────┤
│  • Random Forest                    │
│  • Logistic Regression              │
│  • Support Vector Machine           │
└─────────────────────────────────────┘
          │
          ▼
Model Evaluation & Comparison
          │
          ▼
┌─────────────────────────────────────┐
│      Additional Prediction Tasks    │
├─────────────────────────────────────┤
│  • Injury Location Prediction       │
│  • Recovery Period Prediction       │
└─────────────────────────────────────┘
          │
          ▼
Final Performance Analysis
```

---

# 🤖 Machine Learning Tasks

## 1️⃣ Injury Risk Prediction

The primary task is to predict whether an athlete is at risk of injury.

### Models Used

- Random Forest Classifier
- Logistic Regression
- Support Vector Machine (SVM)

### Evaluation Metrics

The classification models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

---

## 📈 Model Performance Comparison

| Model | Accuracy | F1 Score | ROC-AUC |
|---|---:|---:|---:|
| Random Forest | 89.50% | 85.91% | 95.08% |
| 🏆 Logistic Regression | **98.50%** | **98.04%** | **99.97%** |
| Support Vector Machine | 94.50% | 92.90% | 99.60% |

### 🏆 Best Performing Model

**Logistic Regression** achieved the highest performance for injury risk prediction.

- Accuracy: **98.5%**
- F1 Score: **98.04%**
- ROC-AUC Score: **99.97%**

> The high performance should be interpreted in the context of the synthetic dataset and its generated feature relationships.

---

# 📍 Injury Location Prediction

The project also performs multiclass classification to predict the potential location of an injury.

### Result

- Accuracy: **28.38%**

Injury location prediction is a more challenging task because multiple injury categories may share similar athlete characteristics.

This highlights the complexity of multiclass prediction and the potential need for additional features and real-world data.

---

# ⏳ Recovery Period Prediction

A regression model is used to estimate the expected recovery period.

### Model Performance

| Metric | Score |
|---|---:|
| RMSE | 6.93 Days |
| MAE | 5.20 Days |
| R² Score | 0.5354 |

The regression model demonstrates moderate predictive capability for estimating recovery periods.

---

# 📊 Exploratory Data Analysis

The project includes Exploratory Data Analysis to understand patterns and relationships within the dataset.

Analysis includes:

- Feature distributions
- Injury risk distribution
- Correlation analysis
- Feature importance analysis
- Model performance comparison
- Confusion matrices
- ROC curves
- Regression performance analysis

---

# 🔍 Feature Analysis

The project analyzes the importance of athlete-related factors in predicting injury outcomes.

Some important factors explored include:

- Previous Injuries
- Training Load
- Recovery Time
- Muscle Fatigue
- Joint Flexibility
- Hydration Level

Feature importance analysis helps identify which variables contribute most significantly to the prediction models.

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Computing |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |
| Jupyter Notebook | Development Environment |

---

# 📂 Project Structure

```text
Sports-Injury-Prediction-ML/
│
├── README.md
├── sports_injury_prediction.ipynb
├── sports_injury_dataset.csv
└── requirements.txt
```

---

# ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/Aditya-Kusale/Sports-Injury-Prediction-ML.git
```

### Navigate to the project directory

```bash
cd Sports-Injury-Prediction-ML
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
sports_injury_prediction.ipynb
```

---

# 📦 Requirements

Create a `requirements.txt` file containing:

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
jupyter
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

# 📌 Key Findings

- Multiple Machine Learning models were successfully implemented and compared.
- Logistic Regression achieved the strongest performance for injury risk prediction on the synthetic dataset.
- Injury location prediction proved significantly more challenging due to the multiclass nature of the problem.
- Recovery period prediction demonstrated moderate predictive performance.
- Feature analysis provided insights into factors associated with injury-related outcomes.
- Comparing multiple algorithms provides a broader understanding of model performance.

---

# ⚠️ Limitations

This project has several limitations:

- The dataset is synthetically generated.
- Results should not be interpreted as clinical or medical predictions.
- High classification performance may reflect relationships introduced during synthetic data generation.
- Real-world injury prediction requires larger and more diverse datasets.
- Important factors such as biomechanics, medical history, sport type, and longitudinal training data are not fully represented.

This project is intended primarily as an **educational demonstration of an end-to-end Machine Learning workflow**.

---

# 🚀 Future Improvements

Potential improvements include:

- Using real-world sports injury datasets.
- Performing hyperparameter optimization using GridSearchCV.
- Applying k-fold cross-validation.
- Investigating class imbalance techniques such as SMOTE.
- Adding additional biometric and performance features.
- Experimenting with advanced models such as XGBoost.
- Developing an interactive Streamlit dashboard.
- Deploying the model as a web application.
- Integrating real-time athlete performance data.

---

# ✨ Project Highlights

- ✅ End-to-End Machine Learning Workflow
- 📊 Exploratory Data Analysis
- 🤖 Multiple Classification Models
- 🎯 Binary Classification
- 📍 Multiclass Classification
- 📈 Regression Analysis
- 🔍 Feature Importance Analysis
- 📉 ROC Curve Analysis
- 📊 Confusion Matrices
- 🏆 Model Performance Comparison

---

# 👨‍💻 Author

**Aditya Kusale**

GitHub: https://github.com/Aditya-Kusale

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐!
