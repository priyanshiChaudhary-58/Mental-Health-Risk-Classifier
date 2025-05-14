# 🧠 Mental Health Risk Classifier

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange)

This project uses machine learning to classify students into **Low**, **Medium**, **High**, or **Critical** mental health risk categories based on their responses to a mental health survey. It aims to assist early detection of **depression**, **anxiety**, and **panic attacks**, helping institutions support student well-being proactively.

---

## 📊 Dataset

- **Name:** `Student Mental health.csv`
- **Features:** Age, CGPA, academic year, course, mental health conditions, etc.

---

## 🔍 Feature Engineering

- Created a custom `risk_level` label:
  - **Low**: No condition
  - **Medium**: One condition
  - **High**: Two conditions
  - **Critical**: All three – Depression, Anxiety, Panic Attack
- Mapped CGPA ranges to numeric values
- Extracted numerical values from text-based columns
- Label-encoded and one-hot encoded categorical features

---

## 🤖 Models Used

- Logistic Regression – Best performing (💯 Accuracy: 71.43%, Precision: 80.45%)
- Decision Tree – Easy interpretability
- Random Forest – Best performing (💯 Accuracy: 71.43%, Precision: 80.45%)

---

## 📦 Output

- Best model (Random Forest) exported as `model.pkl` for deployment or further use.

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Confusion Matrix (visualized using `ConfusionMatrixDisplay`)

---

## 🛠️ Tech Stack

- **Languages:** Python
- **Libraries:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `joblib`

---

## 🚀 How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
python Mental-Health-Risk-Classifier.py
