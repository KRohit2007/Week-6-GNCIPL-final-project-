 Week-6-GNCIPL-final-project-
[27/10, 20:32] Kavya Intern GNCIPL: # Insurance Fraud Detection — Exploratory Data Analysis (EDA)

 Project Context

This repository contains the Exploratory Data Analysis (EDA) step of our group project on insurance fraud detection. EDA is a critical intermediary step following data acquisition and before feature engineering, modeling, and deployment.

---

 Objective

The goal of this step is to thoroughly understand the dataset characteristics, detect anomalies, identify relationships between variables, and gain insights that will guide subsequent feature engineering and model building.

---

Files Included

- **notebooks/fraud_detection_modelling.ipynb**  
  Jupyter notebook containing detailed data exploration, summary statistics, missing data checks, and visualizations.

- **data/nhic-1.csv**  
  Dataset comprising insurance claim records used for EDA.

---

 Key Activities

 1. Data Loading and Initial Inspection

- Loaded the dataset and inspected basic structure using commands such as `.head()`, `.info()`, and `.describe()`.
- Verified column data types and checked for missing values to validate data completeness.

 2. Statistical Summary

- Computed descriptive statistics for numerical columns to understand distributions, means, medians, ranges, and anomalies.
- Analyzed categorical data distributions to understand class balance and categorical feature diversity.

 3. Visual Exploration

- Created histograms and boxplots for numerical features to detect skewness, spread, and outliers.
- Generated count plots for categorical variables to evaluate frequency distributions.
- Examined relationships between features through scatter plots and correlation heatmaps.

 4. Outlier Detection

- Applied Z-score statistical method to identify outliers in key numerical variables.
- Visualized outliers and extreme values to assess their impact on data quality.
- Documented outliers to inform filtering decisions in feature engineering.

---

 Insights Gained

- No missing values found, confirming dataset completeness.
- Certain financial columns (e.g., bill amount) exhibited skewness with prominent outliers.
- Strong positive correlations observed between bill amount, claimed amount, and amount paid.
- Smokers tend to have significantly higher medical bills.
- Regional differences in claim patterns were apparent.
- Temporal aspects such as the time delay between application and claim were identified as potential predictive features.

---

 How to Run the Notebook

1. Install required Python packages (e.g., pandas, matplotlib, seaborn).
2. Open the notebook in Jupyter and run cells sequentially to reproduce visualizations and tables.
[27/10, 20:32] Kavya Intern GNCIPL: pip install pandas matplotlib seaborn jupyter
jupyter notebook notebooks/fraud_detection_modelling.ipynb
[27/10, 20:33] Kavya Intern GNCIPL: ---

Notes for Next Steps

- Insights from this analysis informed the feature engineering and modeling steps.
- Particular attention should be paid to handling outliers and exploiting strong feature correlations during model building.

---

Author
K Rohit 

  

---

 Acknowledgments

Dataset provided by National Health Insurance Corporation (NHIC).  
This project is a collaborative effort between team members focusing on different pipeline stages.
