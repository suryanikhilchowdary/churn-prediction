🏥 Healthcare Patient Stay Prediction

Predicting how long a patient will stay in hospital using Machine Learning and Deep Learning.

📊 Results
| Model | Accuracy |
|-------|----------|
| Logistic Regression | 38.05% |
| Random Forest | 38.50% |
| Deep Learning (Keras) | **41.95%** ✅ |

 🛠️ Tech Stack
- **Python** — Data processing & modeling
- **Pandas, NumPy** — Data manipulation
- **Scikit-learn** — ML models & preprocessing
- **TensorFlow / Keras** — Deep Learning
- **Matplotlib, Seaborn** — Visualizations
- **Power BI** — Interactive dashboard
- **Git & GitHub** — Version control

📁 Project Structure
churn-prediction/
├── data/healthcare/       ← Raw dataset
├── notebooks/             ← Jupyter notebooks
│   ├── 01_EDA.ipynb
│   ├── 02_Preprocessing.ipynb
│   ├── 03_ML_Models.ipynb
│   ├── 04_DeepLearning.ipynb
│   └── 05_Evaluation.ipynb
├── models/                ← Saved trained model
├── outputs/               ← CSV exports for Power BI
├── reports/               ← Charts & Power BI dashboard
└── requirements.txt
🚀 How to Run
1. Clone the repo
2. Install dependencies: `pip install -r requirements.txt`
3. Run notebooks in order (01 → 05)
4. Open Power BI dashboard in `reports/`

📈 Dashboard
Built in Power BI showing:
- Model accuracy comparison
- Patient stay distribution
- Actual vs predicted stay
- Key KPI metrics

👤 Author
Surya Nikhil Chowdary
