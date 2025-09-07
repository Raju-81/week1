# Predictive Modeling of Lead Contamination in Drinking Water

## Project Overview
This project analyzes drinking water sampling results to classify whether water is **Safe** or **Unsafe**
based on lead concentrations compared to the Maximum Contaminant Level (MCL).

Using the dataset `lead_in_drinking_water_sampling_results.csv`, we perform data preprocessing, exploratory data analysis,
and train a **Logistic Regression model** to predict unsafe lead levels in drinking water.

## Dataset
- **Source:** Drinking water sampling results dataset (CSV format)
- **Key Columns:**
  - `Result`: Measured lead concentration
  - `MCL`: Maximum Contaminant Level threshold
  - Other metadata: School, District, Sample Date, etc.

## Workflow
1. Data preprocessing (handling missing values, encoding categorical features)
2. Exploratory Data Analysis (pairplots, correlation heatmap)
3. Classification target creation: `Unsafe = (Result >= MCL)`
4. Model training: Logistic Regression (with imputation)
5. Evaluation: Accuracy, Classification Report, Confusion Matrix
6. Model saving with `joblib`

## Results
- Accuracy score and classification metrics reported
- Visualizations:
  - Pairplot of numeric features
  - Correlation heatmap (Magma colormap)
  - Confusion matrix (Magma colormap)

## Files Generated
- `logistic_regression_lead_model.joblib` → Saved trained model
- `imputer_lead_model.joblib` → Saved imputer for missing values
- Notebook/code script for full pipeline

## Requirements
- Python 3.x
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- joblib

## Usage
1. Place the dataset in your working directory.
2. Run the notebook or script to reproduce results.
3. Use the saved model for predictions on new data.

---
**Title:** Predictive Modeling of Lead Contamination in Drinking Water  
**Author:** [Your Name]  
