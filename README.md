# 🚢 Titanic Survival Prediction using Decision Tree

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/ML-scikit--learn-orange)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

This project uses a **Decision Tree Classifier** to predict passenger survival on the Titanic based on selected features such as age, fare, and class. It also includes a simple prediction for a hypothetical passenger and a scatter plot to visualize actual vs. predicted outcomes.

---

## 📁 Project Files

- `titanic.csv` – Dataset with passenger information (must be placed in the same directory)
- `titanic_survival_decision_tree.py` – Python script for training, testing, and predicting
- `README.md` – Project documentation

---

## 📊 Dataset Overview

The Titanic dataset contains demographic and travel information of passengers. The target variable is:

- `Survived`: 1 if the passenger survived, 0 otherwise

### Features used in this model:

| Feature   | Description                                |
|-----------|--------------------------------------------|
| Pclass    | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Sex       | Gender (encoded: male = 0, female = 1)      |
| Age       | Age in years (missing values imputed)       |
| SibSp     | Number of siblings/spouses aboard          |
| Parch     | Number of parents/children aboard          |
| Fare      | Ticket fare (missing values imputed)        |

---

## ⚙️ Model Details

- **Model**: Decision Tree Classifier
- **Library**: `scikit-learn`
- **Evaluation Metric**: Accuracy

---

## ✅ Sample Output


> The model is trained using 80% of the data and tested on the remaining 20%.

---

## 📈 Visualization

A scatter plot compares actual survival outcomes with predicted outcomes.

![Actual vs Predicted](assets/titanic_actual_vs_predicted.png) <!-- Add this image manually if desired -->

---

## 🧪 Example: New Passenger Prediction

The script includes an example prediction for a new passenger with the following features:

- Class: 2nd
- Gender: Female
- Age: 30
- Siblings/Spouses aboard: 0
- Parents/Children aboard: 0
- Fare: 10

Prediction output:
```bash
Prediction for new passenger: Survived
