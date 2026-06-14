# 🚆 Railway Ticket Confirmation Predictor

An AI-powered Railway Ticket Confirmation Prediction System that estimates the probability of a waitlisted train ticket getting confirmed.

The project uses Machine Learning (LightGBM) along with Explainable AI (SHAP and LIME) to provide both predictions and understandable explanations for users.

---

## 📌 Features

- Predicts ticket confirmation probability
- Interactive Streamlit web application
- Uses LightGBM for accurate classification
- SHAP-based feature importance analysis
- LIME-based local explanations
- Human-readable prediction reasoning
- Visualization of SHAP vs LIME feature contributions

---

## 🛠️ Tech Stack

### Machine Learning
- LightGBM
- Scikit-Learn
- Pandas
- NumPy

### Explainable AI (XAI)
- SHAP
- LIME

### Visualization
- Matplotlib

### Deployment
- Streamlit

## 📂 Project Structure

```text
Railway-Ticket-Confirmation-Predictor/
│
├── app.py
├── preprocess.py
├── train.py
├── ticket_model.pkl
├── cleaned_rtc_data.csv
├── Final_RTC.csv
├── requirements.txt
└── README.md
```

---

## 🔄 Project Workflow

```text
Raw Railway Dataset
        │
        ▼
  Data Preprocessing
        │
        ▼
 Feature Engineering
        │
        ▼
   Model Training
        │
        ▼
   Saved Model (.pkl)
        │
        ▼
 Streamlit Application
        │
        ▼
 Prediction + XAI Analysis
```

---


## 🤖 Model Training

The project uses:

- LightGBM Classifier
- RandomizedSearchCV for Hyperparameter Optimization
- Train-Test Split Validation

Hyperparameters optimized:

- n_estimators
- learning_rate
- num_leaves
- max_depth

---

## 🔍 Explainable AI

### SHAP

SHAP helps understand:

- Which features increase confirmation chances
- Which features decrease confirmation chances
- Global feature importance

### LIME

LIME provides:

- Local explanations for individual predictions
- Feature contribution analysis for specific users
