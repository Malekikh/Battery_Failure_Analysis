# 🔋 Battery Failure Prediction – Synthetic Dataset

This project explores predictive modeling on a **synthetic dataset** simulating battery failure scenarios using operational variables such as temperature, pressure, cycle count, and voltage. The goal is to identify potential failures in advance using classification techniques.


---

## 📊 Dataset Overview

| Feature        | Description                         | Unit              |
|----------------|-------------------------------------|-------------------|
| `Temperature`  | Operating temperature               | °C (Celsius)      |
| `Pressure`     | Internal or chamber pressure        | kPa               |
| `Cycle_Count`  | Number of charge/discharge cycles   | Count             |
| `Voltage`      | Voltage of the battery              | V (Volts)         |
| `Failed`       | Failure status                      | Binary (0 = No, 1 = Yes) |

---

## 🔍 Analysis Summary

Both **Python (scikit-learn)** and **Minitab** were used to explore and model the data using:
- **Exploratory Data Analysis (EDA)** and visualization
- **Regression modeling** (Logistic Regression)
- **Decision Tree classification**

![image](https://github.com/user-attachments/assets/3aaf3948-5830-4122-a401-13c3d87445d7)
![image](https://github.com/user-attachments/assets/f3c336b3-4e1c-4cc4-a1f0-e505c99fe20f)
![image](https://github.com/user-attachments/assets/f5b5a35a-dfaf-4d1a-b9bf-6f9194c5708e)
![image](https://github.com/user-attachments/assets/900dc955-e73b-4c4f-9445-7597d20b5a6b)

---
## 📊 Feature Impact Summary

| Feature         | Coefficient Sign | Interpretation                                                                 |
|----------------|------------------|--------------------------------------------------------------------------------|
| 🔥 Temperature | ➕ Positive       | ⬆️ Higher temperature → ⬆️ Higher likelihood of failure (high importance)     |
| ⚡ Voltage      | ➖ Negative       | ⬆️ Higher voltage → ⬇️ Lower likelihood of failure (high importance)          |
| 🧯 Pressure     | ➕ Positive       | ⬆️ Higher pressure → ⬆️ Higher likelihood of failure (moderate importance)    |
| 🔁 Cycle Count | ~ 0              | ➖ Little or no effect on failure in this model                                 |

---

## 🧠 Modeling Results

| Model              | Tool      | Accuracy   |
|-------------------|-----------|------------|
| Logistic Regression | Python    | 82%       |
| Logistic Regression | Minitab    | 87%       |
| Decision Tree       | Minitab   | 99.5%     |
| Decision Tree       | Python    | 100%       |

## Confusion Matrices
![image](https://github.com/user-attachments/assets/8355be8c-e1e4-4081-9fb4-a5545aa93eed)
![image](https://github.com/user-attachments/assets/c2dc6039-6ea1-4a96-a78b-dcd9b5eb53e8)

### ✅ Conclusion:
1) The **Decision Tree model** outperformed other approaches, showing **very high prediction accuracy** in both tools. This indicates that the features are highly separable and decision tree logic fits the data structure well.
2) Temperature and voltage are the most critical factors influencing battery failure, with high temperatures increasing and high voltages decreasing the likelihood of failure, while pressure has a moderate effect and cycle count shows minimal impact.

---

## 🛠️ Tools & Libraries

- Python (`pandas`, `matplotlib`, `seaborn`, `scikit-learn`)
- Minitab (Decision Tree Classifier, Regression Modeling)
- GitHub (for version control and sharing)

---

## 📌 Next Steps (optional ideas)
- Add noise or variability to test model robustness
- Try ensemble models (Random Forest, XGBoost)
- Explore feature importance and SHAP values for model explainability

---

## 👩‍🔬 Author

**Khatereh Maleki**  
Materials Engineer | Failure Analysis | Corrosion | Data Enthusiast  




