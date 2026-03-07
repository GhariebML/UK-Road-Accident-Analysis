---

# 🚦 UK Road Accident Data 2021 — End-to-End EDA & Baseline ML

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Scikit-Learn](https://img.shields.io/badge/ML-Scikit--Learn-yellow)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

# 📌 Project Overview

This project presents a **complete end-to-end data science workflow** applied to the **UK Road Safety Dataset (2021)**.
The analysis focuses on identifying patterns in road accidents and building **machine learning models to predict accident severity**.

The project includes:

* Data cleaning and preprocessing
* Feature engineering
* Exploratory Data Analysis (EDA)
* Statistical testing
* Machine learning modeling
* Model evaluation and comparison

The objective is to **extract insights that can support road safety improvement and accident risk understanding**.

---

# 📊 Dataset Information

| Property        | Value               |
| --------------- | ------------------- |
| Dataset         | UK Road Safety Data |
| Region          | London Districts    |
| Years           | 2021–2022           |
| Records         | 307,973 accidents   |
| Features        | 26                  |
| Target Variable | AccidentSeverity    |

### Target Classes

| Class   | Description    |
| ------- | -------------- |
| Slight  | Minor accident |
| Serious | Serious injury |
| Fatal   | Fatal accident |

---

# 📂 Project Pipeline

```
Data Loading
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Exploratory Data Analysis (EDA)
      ↓
Statistical Testing (Chi-Square)
      ↓
Data Preprocessing
      ↓
Machine Learning Models
      ↓
Model Evaluation & Comparison
```

---

# 🔍 Exploratory Data Analysis (EDA)

### Missing Values

| Column                | Missing % |
| --------------------- | --------- |
| CarriagewayHazards    | 98.24%    |
| WeatherConditions     | 1.97%     |
| RoadType              | 0.50%     |
| RoadSurfaceConditions | 0.10%     |
| Time                  | 0.01%     |

---

### Key Insights

Some important findings from the analysis:

• **Slight accidents represent about 85% of total cases**

• **Peak accident hours:**

* 8–9 AM
* 4–6 PM (Rush hours)

• **Darkness conditions increase accident severity**

• **Wet road surfaces are associated with more serious accidents**

• **Urban areas experience the highest accident frequency**

• **Single carriageway roads show the highest accident rates**

---

# 🤖 Machine Learning Models

Six baseline classification models were trained and evaluated using **5-Fold Cross Validation**.

| Model               | Description                    |
| ------------------- | ------------------------------ |
| Logistic Regression | Linear classification baseline |
| Random Forest       | Ensemble tree model            |
| Gradient Boosting   | Boosting algorithm             |
| K-Nearest Neighbors | Distance-based classifier      |
| Decision Tree       | Tree-based model               |
| SVM (RBF Kernel)    | Non-linear classifier          |

---

# 🏆 Best Model

**Random Forest**

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 83.67% |
| Precision | 76.11% |
| Recall    | 83.67% |
| F1 Score  | 78.84% |

### Classification Report

```
Class      Precision  Recall  F1-score
Fatal        0.07      0.01      0.02
Serious      0.21      0.05      0.08
Slight       0.86      0.97      0.91
```

⚠ **Note:** The dataset is **highly imbalanced**, which explains the lower performance on the Fatal and Serious classes.

---

# 📈 Visualizations

The project includes multiple visualizations:

* Accident severity distribution
* Accidents by hour of day
* Accidents by day of week
* Weather conditions vs severity
* Road surface vs severity
* Light conditions vs severity
* Correlation matrix
* Model comparison charts
* Cross-validation performance plots

---

# 🛠 Tech Stack

| Tool         | Purpose                   |
| ------------ | ------------------------- |
| Python       | Programming language      |
| Pandas       | Data manipulation         |
| NumPy        | Numerical computing       |
| Matplotlib   | Data visualization        |
| Seaborn      | Statistical visualization |
| Scikit-learn | Machine learning          |
| SciPy        | Statistical testing       |
| Google Colab | Development environment   |

---

# 🚀 How to Run

## Option 1 — Google Colab

1. Open the notebook in **Google Colab**
2. Run all cells sequentially

```
Runtime → Run All
```

---

## Option 2 — Run Locally

Clone the repository:

```
git clone https://github.com/YOUR_USERNAME/uk-road-accident-eda-ml.git
cd uk-road-accident-eda-ml
```

Install dependencies:

```
pip install -r requirements.txt
```

Run the notebook:

```
jupyter notebook
```

---

# 📁 Repository Structure

```
uk-road-accident-eda-ml/

│
├── UK_Road_Accident_EDA_ML.ipynb
├── README.md
├── requirements.txt
└── assets/
```

---

# 🔮 Future Improvements

* Handle class imbalance using **SMOTE**
* Hyperparameter tuning using **GridSearchCV**
* Test advanced models such as **XGBoost / LightGBM**
* Add **geospatial accident analysis**
* Build a **Streamlit dashboard**
* Apply **SHAP model explainability**

---

# 👨‍💻 Author

**Mohamed Gharieb**

AI & Data Science Specialist
Applied Machine Learning | Data Analytics | Python | SQL

🔗 GitHub
[https://github.com/YOUR_USERNAME](https://github.com/GhariebML)

🔗 LinkedIn
[https://linkedin.com/in/YOUR_LINKEDIN](https://www.linkedin.com/in/ghariebml/)

---

# 📄 License

This project is licensed under the **MIT License**.

---

⭐ If you found this project useful, consider **starring the repository**.

---

## Next step (important)

After adding the README:

```bash
git add README.md
git commit -m "Add professional README"
git push
```

---

💡 If you want, I can also show you **3 tricks to make your GitHub project look 10× more professional (used by top data scientists)**:

* auto images in README
* project preview
* animated charts.
