# Predicting Gold Recovery from Ore Using Machine Learning
This project predicts gold recovery from ore using machine learning. It analyzes mineral concentrations and process data to build models that support efficient mining operations. Gradient Boosting achieved the best performance with a sMAPE of 11.39.



This project focuses on developing a machine learning model to predict gold recovery rates from gold ore during various stages of processing. It was built for a company specializing in efficiency solutions for the heavy industry. The model is designed to support smarter decision-making in gold extraction by forecasting recovery performance based on process parameters and mineral concentrations.

---

## 📊 Overview

Gold mining operations rely on accurate predictions of recovery rates to maximize yield and minimize waste. In this project, we used industrial datasets to:
- Preprocess and analyze raw data from multiple processing stages.
- Explore how concentrations of gold, silver, and lead change during purification.
- Build and evaluate machine learning models for recovery prediction.

---

## 🧾 Dataset

The dataset includes three main stages of processing:
- **Raw feed**
- **Rougher output**
- **Final concentrate**

Each dataset contains:
- Mineral concentrations (Au, Ag, Pb)
- Physical parameters (airflow, temperature, pH, particle size)
- Time-series data aligned with recovery outcomes

---

## 🧹 Data Preprocessing

Key preprocessing steps:
- Handled missing values using forward fill (time series-aware)
- Identified and removed anomalies (e.g., near-zero or invalid concentration totals)
- Ensured train/test consistency in feature distributions (e.g., particle sizes)

---

## 📈 Exploratory Analysis

- Tracked mineral concentration trends across processing stages
- Compared feed particle size distributions between training and test sets
- Analyzed total substance concentrations to detect outliers

---

## 🤖 Modeling

### Models Tested:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor ✅ *Best performing*
- XGBoost Regressor

### Evaluation Metric:
- **sMAPE (Symmetric Mean Absolute Percentage Error)**

### Best Result:
- **Gradient Boosting**: `sMAPE = 11.39`

---

## 🧠 Key Learnings

- Real-world industrial datasets require domain-specific cleaning and validation.
- sMAPE is an effective metric for evaluating predictions in relative percentage terms.
- Gradient Boosting is well-suited for structured regression tasks with complex relationships.

---

## 🚀 How to Run

1. Clone the repository:

