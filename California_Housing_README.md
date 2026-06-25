# 🏡 California Housing Price Prediction

A machine learning project comparing multiple regression models to predict median house values, achieving an **R² score of 0.80** with the best-performing model.

Built as part of the MSc Advanced Data Science programme at the University of Exeter.

---

## 📋 Project Overview

Housing price prediction is a classic regression problem in applied machine learning. This project trains and benchmarks **four different ML models** on the California Housing dataset, applying a full preprocessing pipeline and evaluating each model to identify the best approach.

---

## 🎯 Results

| Model | R² Score |
|-------|----------|
| Linear Regression | — |
| Support Vector Regressor (SVR) | — |
| Multi-Layer Perceptron (MLP) | — |
| **Random Forest Regressor** | **0.80** ✅ |

> Best model achieved an R² of **0.80**, meaning the model explains 80% of variance in housing prices.

---

## 🗂️ Dataset

**California Housing Dataset** — available directly via `sklearn.datasets.fetch_california_housing()`

- **Samples:** 20,640
- **Features:** 8 (median income, house age, average rooms, average bedrooms, population, average occupancy, latitude, longitude)
- **Target:** Median house value (in $100,000s)
- **Source:** U.S. Census data for California districts (1990)

---

## 🔧 Methodology

### 1. Data Preprocessing
- **Missing value imputation** — handled null/NaN entries to ensure clean input data
- **Feature scaling** — standardised numerical features using `StandardScaler` for distance-sensitive models (SVR, MLP)
- **One-hot encoding** — encoded any categorical variables for compatibility with all models

### 2. Models Trained
| Model | Key Characteristic |
|-------|--------------------|
| Linear Regression | Baseline; assumes linear relationships |
| Random Forest Regressor | Ensemble of decision trees; handles non-linearity |
| Support Vector Regressor (SVR) | Kernel-based; effective in high-dimensional space |
| MLP Neural Network | Feedforward network; captures complex patterns |

### 3. Evaluation
- **R² Score** (coefficient of determination) used as primary metric
- All four models benchmarked on the same train/test split for fair comparison
- Best model selected based on held-out test set performance

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| scikit-learn | Models, preprocessing, and evaluation |
| TensorFlow / Keras | MLP neural network implementation |
| NumPy / pandas | Data manipulation and analysis |
| Matplotlib / Seaborn | Visualisation of distributions and results |

---

## 📁 Project Structure

```
california-housing-prediction/
│
├── california_housing.ipynb   # Main Colab notebook
├── README.md                  # Project documentation
└── requirements.txt           # Dependencies
```

---

## 🚀 Getting Started

### Run in Google Colab
Click the badge below to open the notebook directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_LINK_HERE)

### Run Locally
```bash
# Clone the repository
git clone https://github.com/BhaveshBhargv/california-housing-prediction.git
cd california-housing-prediction

# Install dependencies
pip install -r requirements.txt

# Open the notebook
jupyter notebook california_housing.ipynb
```

---

## 📦 Requirements

```
scikit-learn
tensorflow>=2.x
numpy
pandas
matplotlib
seaborn
jupyter
```

---

## 🎓 Academic Context

- **Programme:** MSc Advanced Data Science, University of Exeter
- **Type:** Coursework Project
- **Key Concepts:** Regression, Ensemble Methods, Neural Networks, Preprocessing Pipelines, Model Benchmarking

---

## 👤 Author

**Bhavesh Bhargava**
[LinkedIn](https://www.linkedin.com/in/bhavesh-bhargava-80ab2a10b/) · [GitHub](https://github.com/BhaveshBhargv/)
