# DS-A3 Regression Baseline and Diagnostics

## 1. Project Overview

This project focuses on regression modeling and model diagnostics using the diabetes dataset. The main goal is to build a baseline regression model, compare different model settings, and evaluate the model performance.

The project also uses diagnostic plots to understand prediction errors and identify possible problems with the model.

## 2. Project Structure

The repository contains the following files and folders:

- `data/` - Contains the diabetes dataset.
- `Result/` - Contains diagnostic plots and CSV files with analysis results.
- `report/` - Contains the project report in DOCX and PDF formats.
- `DS_A3_Regression_Baseline_Diagnostics.ipynb` - Main notebook for the analysis.
- `DS_A3_Regression_Baseline_Diagnostics.executed.ipynb` - Notebook with executed results.
- `AI_USE_LOG.md` - Record of AI tool usage.
- `CLAIM_BOUNDARY.md` - Describes the limits of the project claims.
- `README.md` - Project overview and instructions.

## 3. Dataset

The dataset is stored in `data/diabetes.csv`.

It is used to develop and evaluate regression models. The data is analyzed to compare predicted values with actual values and to study the errors made by the models.

## 4. Method

The project follows these main steps:

1. Load and explore the dataset.
2. Prepare the data for regression analysis.
3. Build a baseline regression model.
4. Compare model performance and tune the Ridge regression model.
5. Analyze residuals and other diagnostic measures.
6. Generate plots and summary tables.
7. Discuss the results and limitations.

## 5. Results

The `Result/` folder contains the following visualizations:

- `01_actual_vs_predicted.png` - Compares actual and predicted values.
- `02_residuals_vs_fitted.png` - Shows residuals against fitted values.
- `03_residual_qq.png` - Examines the distribution of residuals.
- `04_learning_curve.png` - Shows model performance as the training data increases.
- `05_cooks_distance.png` - Helps identify potentially influential observations.
- `06_critical_slices.png` - Shows model performance for selected data groups.
- `07_model_comparison_table.png` - Presents a comparison of different models.
- `08_diagnostics_summary_table.png` - Summarizes the diagnostic results.

The folder also contains CSV files with model comparison results, diagnostic summaries, critical slice metrics, and Ridge tuning results.

## 6. How to Run

### Requirements

- Python 3.11 or later
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- scikit-learn
- nbconvert

### Install the Required Libraries

Run the following command in your terminal:

```bash
pip install pandas numpy matplotlib scikit-learn jupyter nbconvert
```

### Run the Notebook

Open a terminal in the project folder and run:

```bash
jupyter notebook DS_A3_Regression_Baseline_Diagnostics.ipynb
```

Run the notebook cells in order to reproduce the analysis.

To execute the notebook from the terminal, use:

```bash
jupyter nbconvert --to notebook --execute DS_A3_Regression_Baseline_Diagnostics.ipynb --output DS_A3_Regression_Baseline_Diagnostics.executed.ipynb
```

## 7. Report

The `report/` folder contains the project report in two formats:

- `DS-A3- Regression Baseline Diagnostics_Report.docx`
- `DS-A3- Regression Baseline Diagnostics_Report.pdf`

The report explains the analysis, model evaluation, diagnostic results, and main findings.

## 8. Conclusion

This project demonstrates how regression models can be evaluated using performance metrics and diagnostic plots. Comparing models and examining residuals helps provide a better understanding of model performance and its limitations.
