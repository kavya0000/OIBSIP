# Oasis Infobyte Internship Program (OIBSIP)

**Intern:** Poleboina Kavya  
**Track:** Data Analytics  
**Tools:** Python · pandas · NumPy · Matplotlib · Seaborn · scikit-learn · Jupyter Notebook

This repository contains my Data Analytics projects for the Oasis Infobyte Internship Program. Every project is a complete, runnable Jupyter Notebook with written observations after each step, a project README, the dataset and chart screenshots.

---

## Projects

| # | Level / Task | Project | Techniques | Key result |
|---|---|---|---|---|
| 1 | Level 1, Task 1 | [EDA on Retail Sales](DataAnalytics-L1-EDARetailSales) | Descriptive statistics, time-series trends, demographics, correlation heatmap | Items priced 300 or 500 are **39.6% of transactions but 88.4% of revenue** |
| 2 | Level 1, Task 3 | [Cleaning Data (Titanic)](DataAnalytics-L1-CleaningData) | Data quality report, group-median imputation, IQR outlier handling, dtype correction | **866 null values reduced to 0**, with every decision documented |
| 3 | Level 2, Task 2 | [Wine Quality Prediction](DataAnalytics-L2-WineQualityPrediction) | Random Forest, SGD, SVC, stratified split, cross-validation | **Random Forest** recommended; the baseline "always Not good" scores 86.4% accuracy, so models are judged on F1 for good wines |

---

## Project summaries

### 1. EDA on Retail Sales
Analysis of 1,000 retail transactions (total revenue 456,000). Findings include a revenue split driven by price point rather than category, equal spending by gender, higher average spend among younger customers, and a weak Q3 (September is the lowest month). The notebook closes with four actionable business recommendations.

### 2. Cleaning Data (Titanic)
Takes the raw Titanic dataset through a documented cleaning workflow: data quality report, missing-value strategy per column (Age by Pclass and Sex median, Embarked by mode, Cabin replaced by a flag), duplicate check, standardisation, IQR outlier treatment, data type correction and a before-versus-after summary. The cleaned data is saved to a CSV.

### 3. Wine Quality Prediction
Predicts whether a red wine is rated "good" (quality 7 or 8) from 11 chemical measurements. Covers class imbalance, removal of 240 duplicate rows, a stratified 80/20 split, three classifiers, feature importance (alcohol, sulphates and volatile acidity matter most) and a side-by-side comparison with 5-fold cross-validation.

---

## Repository structure

```
OIBSIP/
├── DataAnalytics-L1-EDARetailSales/
│   ├── Poleboina_Kavya_L1_Task1_EDA_RetailSales.ipynb
│   ├── retail_sales_dataset.csv
│   ├── README.md
│   └── screenshots/
├── DataAnalytics-L1-CleaningData/
│   ├── Poleboina_Kavya_Task3.ipynb
│   ├── Titanic-Dataset.csv
│   ├── Titanic_cleaned.csv
│   ├── README.md
│   └── screenshots/
├── DataAnalytics-L2-WineQualityPrediction/
│   ├── Poleboina_Kavya_L2_Task2_WineQuality.ipynb
│   ├── winequality-red.csv
│   ├── wine_quality_processed.csv
│   ├── README.md
│   └── screenshots/
└── README.md
```

---

## How to run any project

1. Clone the repository:
   ```bash
   git clone https://github.com/kavya0000/OIBSIP.git
   cd OIBSIP
   ```
2. Install the libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Open a project folder, start `jupyter notebook`, open the `.ipynb` file and choose **Run All**. The dataset is already in each folder.

---

## Datasets and sources
- **Retail Sales:** retail transactions dataset, 1,000 rows.
- **Titanic:** Kaggle, "Titanic Dataset" by M Yasser H (CC0 Public Domain).
- **Wine Quality:** Cortez et al. (2009), UCI Machine Learning Repository / Kaggle (CC BY 4.0).

---

## About
Completed as part of the Oasis Infobyte Internship Program. Connect with me on [GitHub](https://github.com/kavya0000).
