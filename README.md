# Machine Failure Prediction using Sensor Data

This project involves exploring a dataset of machine sensor readings to understand patterns leading to different types of mechanical failures. The primary goal here is to perform detailed Exploratory Data Analysis (EDA) and extract insights that can be useful for predictive modeling later on.

---

## Dataset Summary

The dataset consists of 10,000 rows with both numerical and categorical features:

- **Sensor Data**: Air temperature, process temperature, rotational speed, torque, and tool wear.
- **Categorical Feature**: Machine type — categorized as L, M, or H.
- **Target Variable**: `Machine_failure` (binary)
- **Additional Labels**: Five binary columns indicating specific failure types — TWF, HDF, PWF, OSF, and RNF.

---

## What’s Done

- Plotted distribution graphs for all sensor values to get a feel of their range and skewness.
- Used box plots and heatmaps to identify outliers and correlated features.
- Analyzed class imbalance in both the overall failure column and individual failure types.
- Created grouped bar charts and KDE plots to visualize relationships between sensor values and failures.
- Observed how machine type correlates with failure frequency.

---

## Key Observations

- **Class Imbalance**: Only about 3.4% of the machines have any failure.
- **Highly Correlated Features**: Air and process temperatures are strongly positively correlated.
- **Failure Type Frequency**: HDF and OSF are the most common, RNF is rare.
- **Torque and Rotational Speed**: Inversely related, which might be useful for modeling.

---

## Tech Stack

- Python (Pandas, NumPy)
- Visualization: Matplotlib and Seaborn
- Jupyter Notebook for EDA

---

## Next Steps

- Encode categorical features and scale numerical ones
- Handle imbalance using SMOTE or class weights
- Train classification models (Logistic Regression, Random Forest, etc.)
- Evaluate with metrics like ROC-AUC, F1-score, and confusion matrix

---

## Repo Structure

