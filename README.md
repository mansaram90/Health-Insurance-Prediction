# 🏥 Health Insurance Cost Prediction App

A **machine learning–powered Streamlit application** that predicts **health insurance costs** based on user demographics, lifestyle, and medical history.
This project demonstrates **end-to-end ML deployment**, combining **domain knowledge, feature engineering, model selection, and production-ready inference logic**.

🔗 **Live App:**
👉 [https://health-insurance-prediction-manish-learning.streamlit.app/](https://health-insurance-prediction-manish-learning.streamlit.app/)

---

## 🚀 Project Overview

Health insurance pricing depends on multiple interacting factors such as:

* Age and income
* Lifestyle choices (smoking, BMI)
* Medical history and genetic risk
* Insurance plan and employment status

This project translates those **real-world insurance risk factors** into a **machine learning pipeline** and exposes it via an **interactive Streamlit web app**.

---

## 🧠 Machine Learning & Domain Logic

### Key ML Highlights

* **Pre-trained models and scalers** loaded using `joblib`
* Custom **feature preprocessing and encoding**
* **Risk normalisation logic** based on medical history severity


This mirrors real insurance underwriting strategies where risk behaves differently across age groups.
The logic is implemented in `prediction_helper.py` 

---

## 🧩 Feature Engineering & Risk Modelling

### Medical Risk Normalisation

Medical history is converted into a **numerical risk score**, then normalised to a 0–1 range.

Example:

* Diabetes → higher risk
* Heart disease → highest risk
* No disease → zero risk

This ensures **medical conditions influence predictions in a controlled, interpretable way** rather than raw categorical inputs.

---

## 🖥️ Application Interface (Streamlit)

The Streamlit app (`main.py`) provides:

* Structured input forms for all insurance-relevant variables
* Clean grid-based UI layout
* One-click prediction output

Key inputs include:

* Age, income, dependants
* BMI category and smoking status
* Employment status and region
* Medical history and insurance plan

Implemented in `main.py` 

---

## 📂 Project Structure

```
├── main.py
│   └── Streamlit UI and user input handling
│
├── prediction_helper.py
│   ├── Risk score calculation
│   ├── Feature encoding & scaling
│   ├── Age-based model routing
│   └── Final prediction logic
│
├── artifacts/
│   ├── model_young.joblib
│   ├── model_rest.joblib
│   ├── scaler_young.joblib
│   └── scaler_rest.joblib
│
└── README.md
```

---

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **Scikit-learn**
* **Joblib**
* **Streamlit**

---

## 💡 What This Project Demonstrates

✔ Strong **domain understanding** of insurance risk factors
✔ Practical **ML feature engineering**
✔ Clean separation of **UI, preprocessing, and inference logic**
✔ Real-world **deployment mindset**, not just notebook modelling
✔ Recruiter-ready **end-to-end ML project**

---

## 📌 Future Improvements

* Add explainability (feature impact per prediction)
* Store prediction history
* Improve UI with charts and risk bands
* Retrain with larger real-world datasets

---

## 👤 Author

**Manish Pareek**
Machine Learning & Applied Data Science Enthusiast

If you are a **recruiter or hiring manager**, feel free to explore the live app and the codebase.


