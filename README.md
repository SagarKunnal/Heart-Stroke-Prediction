# ❤️ Heart Stroke Prediction App

An interactive Machine Learning web application built using **Streamlit** and **K-Nearest Neighbors (KNN)** to predict heart disease risk based on clinical health parameters.

---

## 📌 Overview

Cardiovascular diseases are one of the leading causes of health complications globally. Early detection and risk assessment can significantly improve patient outcomes. This project leverages a trained **K-Nearest Neighbors (KNN)** classification model to estimate a person's risk of heart disease based on key medical metrics.

---

## ✨ Features

- 🩺 **User-Friendly Interface**: Intuitive Streamlit Web App with interactive sliders and dropdowns.
- ⚡ **Real-Time Predictions**: Instant classification into **High Risk** or **Low Risk**.
- 📊 **Preprocessing Pipeline**: Integrates pre-trained `StandardScaler` and feature column alignment.
- 🔬 **Data-Driven ML Model**: Built using clinical indicators such as Cholesterol, Max Heart Rate, ST Depression, and Chest Pain types.

---

## 📁 Repository Structure

```
Heart-Stroke-Prediction/
│── app.py                  # Streamlit web application
│── HeartdiseaseFinal.ipynb # Jupyter notebook containing EDA, training & evaluation
│── knn_heart_model.pkl     # Trained KNN classification model
│── heart_scaler.pkl        # Fitted StandardScaler for input normalization
│── heart_columns.pkl       # Feature column order for schema matching
│── requirements.txt        # Python package dependencies
└── README.md               # Project documentation
```

---

## 🛠️ Installation & Local Setup

### 1. Clone the Repository
```bash
git clone https://github.com/SagarKunnal/Heart-Stroke-Prediction.git
cd Heart-Stroke-Prediction
```

### 2. Create & Activate Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit Application
```bash
streamlit run app.py
```
Open your browser and navigate to `http://localhost:8501`.

---

## 📊 Input Clinical Parameters

| Parameter | Description | Valid Range / Categories |
| :--- | :--- | :--- |
| **Age** | Age of the patient | 18 – 100 years |
| **Sex** | Biological Sex | `M` (Male), `F` (Female) |
| **Chest Pain Type** | Type of chest pain experienced | `ATA` (Atypical Angina), `NAP` (Non-Anginal), `TA` (Typical Angina), `ASY` (Asymptomatic) |
| **Resting BP** | Resting Blood Pressure | 80 – 200 mm Hg |
| **Cholesterol** | Serum Cholesterol level | 100 – 600 mg/dL |
| **Fasting BS** | Fasting Blood Sugar > 120 mg/dL | `0` (No), `1` (Yes) |
| **Resting ECG** | Resting Electrocardiogram results | `Normal`, `ST` (ST-T wave abnormality), `LVH` (Left Ventricular Hypertrophy) |
| **Max HR** | Maximum Heart Rate achieved | 60 – 220 bpm |
| **Exercise Angina** | Exercise-induced Angina | `Y` (Yes), `N` (No) |
| **Oldpeak** | ST Depression induced by exercise | 0.0 – 6.0 |
| **ST Slope** | Slope of the peak exercise ST segment | `Up`, `Flat`, `Down` |

---

## ⚠️ Medical Disclaimer

*This application is developed for educational and demonstration purposes only. It does not provide medical diagnoses. Always consult a licensed healthcare professional for medical advice and clinical diagnosis.*
