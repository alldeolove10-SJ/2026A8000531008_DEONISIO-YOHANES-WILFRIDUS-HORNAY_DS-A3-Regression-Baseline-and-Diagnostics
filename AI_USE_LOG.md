# AI_USE_LOG.md

## AI assistance disclosure

AI assistance was used to help organize the DS-A3 workflow, draft reproducible Python code, structure the README/Data Card/Data Dictionary, and edit the short result summary.

## Human verification

I independently checked that:
1. The notebook runs from top to bottom using the frozen local CSV.
2. The train/test split is fixed with `random_state=42`.
3. Ridge alpha is selected only by cross-validation on the training set.
4. The frozen test set is used only for final model comparison.
5. Result CSV files and PNG figures are generated in the `Results/` folder.
6. The numerical values in the short report match the executed notebook outputs.
7. The dataset provenance and SHA-256 hash are recorded.

AI output was not treated as evidence by itself; the analysis results were verified by executing the code and inspecting the generated outputs.
