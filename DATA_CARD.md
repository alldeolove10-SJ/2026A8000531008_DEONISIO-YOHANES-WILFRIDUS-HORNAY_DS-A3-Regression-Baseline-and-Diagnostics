# Data Card — DS-A3 Regression Baseline and Diagnostics

## Dataset
**Name:** Diabetes regression dataset  
**Task:** Predict a quantitative measure of disease progression one year after baseline.

The dataset contains **442 observations**, **10 numeric predictors**, and one target. The predictors are age, sex, body mass index (bmi), average blood pressure (bp), and six serum measurements (s1–s6). The feature variables distributed by scikit-learn are mean-centered and scaled.

## Provenance
- Distribution: scikit-learn `load_diabetes(as_frame=True)`
- Official documentation: https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_diabetes.html
- Dataset description/source information: https://scikit-learn.org/stable/datasets.html
- Original cited work: Efron, Hastie, Johnstone & Tibshirani (2004), *Least Angle Regression*, Annals of Statistics, 32, 407–499.
- DOI: https://doi.org/10.1214/009053604000000067

## Frozen data artifact
- File: `data/diabetes.csv`
- Rows × columns: 442 × 11
- Missing values: 0
- Duplicate rows: 0
- SHA-256: `f16718c1e6602b419193b9a023dbe278ae7f85ff343158813d7040a9f7512dec`
- The CSV is the exact local artifact used by the executed notebook.

## License / use
The dataset is distributed through scikit-learn. The scikit-learn project uses the BSD-3-Clause license; users should also respect any terms associated with the original dataset source. The dataset is used here for educational analysis.

## Intended use
Educational regression benchmarking, diagnostics, and reproducibility exercises.

## Limitations
This is a small, historical dataset. It should not be treated as a clinical deployment dataset. Model performance is not evidence of clinical utility or causal relationships.
