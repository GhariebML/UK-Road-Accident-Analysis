<div align="center">

# 🚦 UK Road Accident Analysis
### End-to-End Data Science: EDA · Statistical Testing · ML Modeling

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)]()

</div>

---

## 📌 Project Overview

A complete end-to-end data science workflow applied to the **UK Road Safety Dataset (307,973 accident records)**. This project identifies patterns in road accidents and builds machine learning models to predict accident severity, delivering actionable insights to support road safety improvements.

### 🎯 Objectives
- Identify key factors that influence accident severity
- Discover temporal and environmental patterns in accident occurrence
- Build and compare 6 baseline ML classification models
- Provide data-driven recommendations for road safety policy

---

## 📊 Dataset

| Property | Value |
|----------|-------|
| Source | UK Road Safety Data |
| Region | London Districts |
| Period | 2021–2022 |
| Records | **307,973 accidents** |
| Features | 26 variables |
| Target | Accident Severity (Slight / Serious / Fatal) |

---

## 🔄 Project Pipeline

```
Data Loading → Data Cleaning → Feature Engineering → EDA
     ↓
Statistical Testing (Chi-Square) → Preprocessing → ML Modeling → Evaluation
```

---

## 🔍 Key EDA Insights

| Finding | Detail |
|---------|--------|
| 🟡 Class Distribution | Slight = **85%** of all accidents |
| ⏰ Peak Hours | 8–9 AM & **4–6 PM** (rush hours) |
| 🌙 Lighting Effect | Darkness increases severity risk |
| 🌧️ Weather Impact | Wet roads correlate with serious accidents |
| 🏙️ Urban vs Rural | Urban areas have highest accident frequency |
| 🛣️ Road Type | Single carriageways show highest accident rates |

---

## 🤖 Machine Learning Models

6 baseline classification models trained with **5-Fold Cross Validation**:

| Model | Type |
|-------|------|
| Logistic Regression | Linear baseline |
| Random Forest 🏆 | Ensemble (Best) |
| Gradient Boosting | Boosting |
| K-Nearest Neighbors | Distance-based |
| Decision Tree | Tree-based |
| SVM (RBF Kernel) | Non-linear |

### 🏆 Best Model: Random Forest

| Metric | Score |
|--------|-------|
| Accuracy | **83.67%** |
| Precision | 76.11% |
| Recall | 83.67% |
| F1 Score | 78.84% |

> ⚠️ **Note:** Dataset is highly imbalanced (85% Slight). SMOTE is planned for v2.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10 | Core language |
| Pandas & NumPy | Data manipulation |
| Matplotlib & Seaborn | Visualization |
| Scikit-learn | ML models |
| SciPy | Statistical testing |
| Google Colab | Development environment |

---

## 🚀 How to Run

**Option 1 — Google Colab (Recommended)**
```
Open the .ipynb file → Runtime → Run All
```

**Option 2 — Run Locally**
```bash
git clone https://github.com/GhariebML/UK-Road-Accident-Analysis.git
cd UK-Road-Accident-Analysis
pip install -r requirements.txt
jupyter notebook
```

---

## 📁 Repository Structure

```
UK-Road-Accident-Analysis/
│
├── UK_Road_Accident_EDA_ML.ipynb   # Main notebook
├── Road Accident Data.xlsx          # Dataset
├── README.md
└── LICENSE
```

---

## 🔮 Future Improvements

- [ ] Handle class imbalance with **SMOTE**
- [ ] Hyperparameter tuning with **GridSearchCV / Optuna**
- [ ] Test **XGBoost / LightGBM**
- [ ] Add **geospatial accident heatmap**
- [ ] Build a **Streamlit interactive dashboard**
- [ ] Apply **SHAP model explainability**

---

## 👨‍💻 Author

<div align="center">

**Mohamed Gharieb**  
*Data Scientist & ML Engineer*

[![GitHub](https://img.shields.io/badge/GitHub-GhariebML-181717?style=flat-square&logo=github)](https://github.com/GhariebML)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-ghariebml-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/ghariebml)

</div>

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

<div align="center">
  <i>If this project helped you, please ⭐ star the repo — it means a lot!</i>
</div>
