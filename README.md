# DS-A3 | Regression Baseline and Diagnostics

This package contains the executable analysis and submission materials for DS-A3.

## Main files
- `DS_A3_Regression_Baseline_Diagnostics.ipynb` — executable notebook
- `DS_A3_Regression_Baseline_Diagnostics.executed.ipynb` — executed notebook with outputs
- `report/DS_A3_Regression_Baseline_Diagnostics_Report.pdf` — 150–300 word result summary
- `DATA_CARD.md` — provenance, integrity, intended use, and limitations
- `data_dictionary.csv` — feature definitions
- `AI_USE_LOG.md` — AI-use disclosure and independent verification
- `requirements.txt` — environment dependencies
- `data/diabetes.csv` — frozen local dataset
- `Results/` — figures, diagnostic tables, model comparison, and tuning results

## Reproduction
Open the notebook in Jupyter and run all cells from top to bottom.

Required packages:
- pandas
- numpy
- matplotlib
- scipy
- scikit-learn
- statsmodels
- jupyter

The notebook reads only `data/diabetes.csv`; it does not require an internet connection.

## Analysis design
1. Freeze a leakage-free 80/20 train-test split (`random_state=42`).
2. Establish a training-mean naive baseline.
3. Fit linear regression and Ridge candidates.
4. Select Ridge alpha using five-fold cross-validation on training data only.
5. Evaluate models once on the frozen test set.
6. Inspect residuals, Q-Q behavior, heteroscedasticity, Cook's distance, learning curves, and a pre-specified BMI slice.
7. State the model boundary and limitations.

## Dataset provenance
The Diabetes dataset is documented by scikit-learn as a regression dataset with 442 samples and 10 predictors:
https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_diabetes.html

Frozen CSV SHA-256:
`f16718c1e6602b419193b9a023dbe278ae7f85ff343158813d7040a9f7512dec`

## Submission note
Submit the notebook, executed notebook, PDF report, data card, data dictionary, AI-use log, frozen data, and Results folder together with the repository URL requested by the course.
