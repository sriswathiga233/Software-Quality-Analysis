SOFTWARE QUALITY INSIGHT — SYNTHETIC PRACTICE DATASET

This dataset was generated for educational use for the Software Quality Insight challenge.
It is synthetic (artificially generated), not real company data and not an official dataset.

Files:
- modules.csv: module-level metadata
- metrics.csv: module-release software metrics
- defects.csv: module-release defect counts and severity
- commits.csv: module-release commit and contributor activity
- releases.csv: release dates and versions

Intentionally included data-quality conditions for practice:
- Missing values in test_coverage and contributors
- A duplicate module-release row in metrics.csv
- An inconsistent module name in metrics.csv
- An extreme complexity value in metrics.csv
- An unmatched defect record for MOD999

Expected workflow:
1. Load all five CSV files in Google Colab.
2. Inspect columns, data types, missing values and duplicates.
3. Standardize module names and clean data.
4. Merge using module and release identifiers.
5. Perform EDA and feature engineering.
6. Train/evaluate a model using a suitable split.
7. Interpret results as patterns in synthetic data only.

Important: Because this is synthetic data, any correlations and model scores are for practice and must not be represented as real-world findings.
