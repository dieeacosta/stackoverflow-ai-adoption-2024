# 📊 AI Tool Adoption Among Developers — Stack Overflow Survey 2024

> Exploratory analysis and predictive modeling of AI tool adoption using the Stack Overflow Developer Survey 2024.

---

## 📌 Project Overview

This project analyzes how technology professionals adopt AI tools based on their role, experience, age, and country. It combines a full EDA with a predictive classification model to answer the question:

**Can we predict whether a developer uses AI tools based on their profile?**

---

## 📂 Dataset

- **Source**: [Stack Overflow Developer Survey 2024](https://survey.stackoverflow.co/)
- **Size**: 65,437 respondents — 114 variables
- **Key variables**: `AISelect`, `AISent`, `AIBen`, `AIThreat`, `AIAcc`, `DevType`, `YearsCode`, `Country`, `Age`, `EdLevel`

---

## 🔍 Analysis Structure

| Section | Description |
|---------|-------------|
| 1.1–1.5 | Data loading, structure, missing values, key variables |
| 1.6–1.7 | Univariate analysis — age, country, languages, AI variables |
| 1.8–2.0 | AI adoption and sentiment by age group |
| 2.1 | AI adoption and trust by experience level |
| 2.2 | AI adoption and sentiment by country |
| 2.3 | AI adoption and sentiment by developer type |
| 3.1–3.3 | Predictive modeling — Logistic Regression, Random Forest, XGBoost |

---

## 💡 Key Findings

- **62%+ of developers** actively use AI tools — adoption is mainstream, not a trend
- **Younger developers adopt more**: 72.3% (0-2 yrs experience) vs 49.2% (20+ yrs)
- **Experience breeds skepticism**: senior developers trust AI less and use it less
- **AI is not seen as a job threat**: only 11-13% consider it a risk across age groups
- **Emerging markets lead**: Ukraine (72.3%), India (67.9%), Brazil (66.0%) outpace USA (54.2%)
- **Front-end developers** show the highest adoption (69.1%) and positive sentiment (75.6%)

---

## 🤖 Predictive Model

**Goal**: Predict whether a developer currently uses AI (`AISelect` = Yes/No)

**Best model**: Logistic Regression v2 — ROC-AUC **0.638**

| Model | Accuracy | F1 | ROC-AUC |
|-------|----------|----|---------|
| Logistic Regression v1 | 0.589 | 0.667 | 0.602 |
| Random Forest v1 | 0.584 | 0.679 | 0.569 |
| Logistic Regression v2 | 0.600 | 0.659 | **0.638** |
| Random Forest v2 | 0.589 | 0.634 | 0.628 |
| XGBoost | 0.596 | 0.644 | 0.633 |

**Key insight**: Developer profile alone has limited predictive power. AI adoption is driven more by individual curiosity and team culture than by age, role, or experience.

---

## 🛠️ Tech Stack

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn, XGBoost
- Jupyter Notebook

---

## 👤 Author

**Diego Acosta** — BI Manager & Data Science student
[LinkedIn](https://www.linkedin.com/in/diego-omar-acosta) | [GitHub](https://github.com/dieeacosta)

---

*MIT License*
