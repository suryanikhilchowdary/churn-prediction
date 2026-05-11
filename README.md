# 🏥 Healthcare Patient Stay Prediction

Predicting hospital length of stay (11 classes) from 318k+ patient records 
using classical ML and deep learning, with results visualized in Power BI.

## 📌 Problem

Hospitals need to forecast patient length of stay to plan bed allocation, 
staffing, and discharge logistics. Accurate predictions reduce overcrowding 
and improve resource utilization. This project builds and compares models 
to predict stay duration across 11 bucketed classes.

## 📊 Dataset

- **Size:** 318,438 patient admission records
- **Target:** Stay duration (11 classes, e.g. "0-10 days", "11-20 days"... "More than 100 days")
- **Features:** Hospital type, ward, admission deposit, severity of illness, age, etc.
- **Source:** [AnalyticsVidhya Healthcare Hackathon] *(update if different)*

## 🛠️ Approach

1. **EDA** — Explored class imbalance, feature distributions, missingness
2. **Preprocessing** — Encoded categoricals, handled missing values, scaled numerics
3. **Baseline ML** — Logistic Regression, Random Forest
4. **Deep Learning** — Keras feedforward network with dropout
5. **Evaluation** — Accuracy, weighted F1, confusion matrix

## 📈 Results

| Model | Accuracy | Weighted F1 |
|---|---|---|
| Majority Class Baseline | ~28% | — |
| Logistic Regression | 38.05% | *(add)* |
| Random Forest | 38.50% | *(add)* |
| **Deep Learning (Keras)** | **41.95%** ✅ | *(add)* |

*11-class problem; random baseline = 9%. Deep learning achieves ~1.5x majority baseline.*

## 📊 Power BI Dashboard

![Dashboard](reports/dashboard.png)

Interactive dashboard built from model predictions for hospital operations teams.

## 🗂️ Project Structure

​```
healthcare-patient-stay-prediction/
├── data/healthcare/              # Raw dataset
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Preprocessing.ipynb
│   ├── 03_ML_Models.ipynb
│   ├── 04_DeepLearning.ipynb
│   └── 05_Evaluation.ipynb
├── models/                       # Saved trained models (.keras)
├── outputs/                      # CSV exports for Power BI
├── reports/                      # Charts & Power BI dashboard
└── requirements.txt
​```

## 🛠️ Tech Stack

**Python · Pandas · NumPy · Scikit-learn · TensorFlow/Keras · Matplotlib · Seaborn · Power BI · Git**

## 🚀 How to Run

​```bash
git clone https://github.com/suryanikhilchowdary/healthcare-patient-stay-prediction.git
cd healthcare-patient-stay-prediction
pip install -r requirements.txt
jupyter notebook
​```

Run notebooks in order: `01` → `02` → `03` → `04` → `05`.
