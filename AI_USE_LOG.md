# AI_USE_LOG.md

## AI assistance disclosure

AI assistance was used to help organize the DS-A3 workflow, draft reproducible Python code.

## I independently checked that:

1. The notebook runs from top to bottom using the frozen local CSV.
2. Ridge alpha is selected only by cross-validation on the training set.
3. The frozen test set is used only for final model comparison.
4. Result CSV files and PNG figures are generated in the `Results/` folder.
5. The numerical values in the short report match the executed notebook outputs.
6. The dataset provenance and SHA-256 hash are recorded.
