# Heart Disease Risk Prediction App

A Streamlit application that uses a saved machine-learning model to estimate heart disease risk from clinical input values. It also includes a page with general heart-health strategies.

> **Educational use only:** This app is not a medical device and does not provide a diagnosis. Do not use its output to make health decisions. For medical advice, consult a qualified healthcare professional.

## Features

- Enter 13 values used by the model: age, gender, chest-pain type, resting blood pressure, cholesterol, fasting blood sugar, resting ECG result, maximum heart rate, exercise-induced angina, ST depression, ST segment slope, major vessels, and thalassemia result.
- View the model's predicted result in the Streamlit interface.
- Browse general healthy-heart strategies.

The input codes and accepted values are shown beside the fields in the app. Fill in every field with a numeric value before requesting a prediction.

## Project contents

- `app.py` — Streamlit user interface and prediction flow.
- `requirements.txt` — Python package dependencies.
- `saved_models/heart_disease_model.sav` — model file loaded by the app.
- `saved_models/dataset/` — dataset and training-related materials.

## Run locally

You need Python and Git installed.

1. Clone the repository and enter its folder:

   ```bash
   git clone https://github.com/Somesh404E/Heart-Disease-Diagnosis.git
   cd Heart-Disease-Diagnosis
   ```

2. Create and activate a virtual environment.

   **Windows PowerShell:**

   ```powershell
   python -m venv .venv
   .venv\Scripts\Activate.ps1
   ```

   **macOS/Linux:**

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install the dependencies and start the app:

   ```bash
   pip install -r requirements.txt
   streamlit run app.py
   ```

Streamlit will print a local URL in the terminal. Open that URL in your browser.

## How to use

1. Open **Heart Disease Prediction** from the sidebar.
2. Enter all requested values using the field labels as a guide.
3. Select **Heart Disease Test Result** to display the model output.
4. Choose **Healthy Heart Strategies** in the sidebar to view general wellness tips.

## Notes

- The app expects the model file at `saved_models/heart_disease_model.sav` relative to `app.py`.
- The prediction depends on the saved model and the values entered. This repository does not establish clinical accuracy or suitability for diagnosis.
- Check the dataset and model terms before redistributing or using them outside this project.
