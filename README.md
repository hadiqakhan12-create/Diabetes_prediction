# 🏥 Medical Prediction: Feature Engineering for Diabetes


## 📌 Project Overview
This project focuses on **Feature Engineering** to improve machine learning predictions for diabetes. Using the Pima Indians Diabetes dataset, I transformed raw medical readings into 10 high-impact synthetic features.

The goal was to move from simple "raw data" to "clinical risk factors" that a doctor would actually use to diagnose a patient.

## 📂 The Dataset
- **Name:** Pima Indians Diabetes Dataset (National Institute of Diabetes and Digestive and Kidney Diseases).
- **Target:** Predict "Outcome" (0 = No Diabetes, 1 = Diabetes).
- **Key Metrics:** Glucose, Blood Pressure, BMI, Insulin, and Family History.

## 🛠️ 10 Engineered Synthetic Features
I developed 10 new features to provide a "Performance Delta" (measured improvement) over raw data:

1.  **Metabolic Risk Score:** A combined score (0-3) based on high Blood Pressure, Glucose, and BMI.
2.  **Glucose-to-Insulin Ratio:** Measures how well the body manages blood sugar.
3.  **BMI Category:** Converts raw BMI into binary "Obese" vs. "Not Obese."
4.  **Blood Pressure Flag:** Binary indicator for clinical hypertension.
5.  **Genetic Risk Exposure:** Multiplies family pedigree by age to see if risk increases as the patient gets older.
6.  **Pregnancy Intensity:** Calculates pregnancies relative to adult years.
7.  **Glucose Stress Level:** A binary flag for glucose levels above the clinical safety threshold.
8.  **Log BMI:** Reduces data skewness for better model training.
9.  **Standardized Skin Fold:** A Z-score for body fat composition.
10. **Senior Status:** Age-based risk indicator (Age > 50).

## 📊 Results & Visualization
- **Before vs. After:** Histograms comparing raw glucose distribution against the newly created Risk Score.
- **Correlation Matrix:** Proving that engineered features (like `risk_score`) have a stronger relationship with the outcome than raw readings.

## 🚀 How to Use
1. Clone the repo: "https://github.com/hadiqakhan12-create/Diabetes_prediction"
2. Run the Jupyter Notebook: `medical.ipynb`
3. Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`

---
**Model and Analysis by Hadiqa Khan**
*Week 3 Internship Task - FutureXcel*
