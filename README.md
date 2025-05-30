# 🔋 Battery Life Prediction using ANN

This project is a Streamlit web application that predicts the **battery life** (ambient temperature-based) using a trained Artificial Neural Network (ANN) model. The app takes in battery parameters and outputs a prediction based on historical data.

## 🚀 Features

- Predict battery life based on:
  - Type of discharge (`charge`, `discharge`, `impedance`)
  - Capacity
  - Re (Equivalent series resistance)
  - Rct (Charge transfer resistance)
- Uses a TensorFlow Keras ANN model for prediction
- Inputs are preprocessed using a saved Scikit-learn scaler and label encoder
- Deployed using Streamlit for easy interaction

## 🧠 Model Details

- Model: ANN trained with TensorFlow (saved as `battery_life_model.h5`)
- Preprocessing:
  - Label Encoding for `type_discharge`
  - Feature Scaling using `StandardScaler`

## 📦 Files

- `battery_life_model.h5` – Trained Keras model
- `scaler.pkl` – Pickled Scikit-learn scaler
- `label_encoder.pkl` – Pickled Scikit-learn LabelEncoder
- `app.py` – Main Streamlit application

## 🛠️ Installation & Running the App

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Janani-N14/Battery_life_prediction_ANN.git
   cd Battery_life_prediction_ANN
