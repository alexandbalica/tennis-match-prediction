# Predicting Tennis Match Outcomes Using Supervised Machine Learning

This project builds a supervised machine learning pipeline to predict ATP tennis match outcomes using point‑level and match‑level performance statistics.
The analysis spans multiple seasons of ATP data and compares several models to identify the most reliable predictors of match success.

---

## 📂 Project Overview

The goal of this project is to evaluate how well different machine learning models can predict match winners based on serve efficiency, return performance, and pressure‑point statistics.
The notebook includes:

- Data loading and preprocessing across multiple seasons  
- Feature engineering focused on efficiency metrics  
- Training and evaluation of three supervised models  
- Hyperparameter tuning using GridSearchCV  
- Feature‑importance analysis across model families  
- Visualization of model behavior and predictive drivers  

---

## 🧠 Models Implemented

Three models were trained and compared:

- **Random Forest Classifier**  
- **Logistic Regression (with scaling pipeline)**  
- **Gradient Boosting Classifier**

A **GridSearchCV‑tuned Random Forest** was also included to optimize performance.

All models were saved to disk to avoid retraining on future runs.

---

## 📊 Key Findings

- Serve‑efficiency metrics (first‑serve points won, second‑serve points won, total serve points won) consistently emerged as the strongest predictors across all models.
- Logistic Regression revealed directional influence through its coefficients.
- Tree‑based models captured nonlinear interactions and concentrated importance in the most predictive features.
- Agreement across models confirmed the strength of the engineered features and explained the similar accuracy levels.

---

## 📁 Repository Contents

- `tennis_match_prediction.ipynb` — Main analysis notebook  
- `data/` — Raw and processed datasets (if included)  
- `models/` — Saved `.pkl` model files  
- `README.md` — Project documentation  

---

## 🚀 How to Run the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/alexandbalica/tennis-match-prediction.git

2. Install dependencies:
pip install -r requirements.txt

3. Open the notebook:
jupyter notebook tennis_match_prediction.ipynb
The notebook automatically loads saved models if available, or trains them once and stores them for future runs.

---

## 📝 Author

Alex Balica
Professional Tennis Coach — Boca Bridges Racquet Club
Machine Learning & Sports Analytics Enthusiast

---

## 📧 Contact

For questions or collaboration opportunities:
alexandbalica@gmail.com
