# Water Potability Classification using SVM

This repository contains a machine learning project to classify whether water is potable (safe to drink) or not, based on various chemical and physical properties. The model uses a **Support Vector Machine (SVM)** classifier trained on the [Water Potability dataset](https://www.kaggle.com/adityakadiwal/water-potability).

---

## Dataset

- **Source:** `water_potability.csv`
- **Target Variable:** `Potability` (0 = Not potable, 1 = Potable)
- **Features:**
  - `ph`
  - `Hardness`
  - `Solids`
  - `Chloramines`
  - `Sulfate`
  - `Conductivity`
  - `Organic_carbon`
  - `Trihalomethanes`
  - `Turbidity`

---

## Data Preprocessing

- Handled missing values:
  - Replaced missing values in `ph`, `Sulfate`, and `Trihalomethanes` with their **median**.
- Split data into **training** and **testing** sets (80/20 split).

---

## Model

- **Algorithm:** Support Vector Classifier (`SVC`) from Scikit-learn
- **Accuracy Achieved:** ~62.8% on test data

---

## Evaluation Metric

- **Accuracy Score:** `0.628`

> This model could benefit from hyperparameter tuning, feature scaling, and advanced ensemble techniques.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/water-potability-svm.git
   cd water-potability-svm
