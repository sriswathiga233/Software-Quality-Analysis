# Software Quality Insight

### Software Defect Analysis and Prediction Using Machine Learning

## 📌 Project Overview

Software Quality Insight is a data science and machine learning project designed to analyze software quality metrics and identify patterns associated with software defects across modules and releases.

The project examines factors such as code complexity, coupling, code churn, test coverage, module size, commit activity, and contributor count to understand how they relate to defect frequency. A Random Forest Regressor is used to estimate defect counts and support data-driven testing and code-review prioritization.

**Note:** This project uses a synthetically generated dataset for educational and experimental purposes. The data does not represent a real company or production software system.

## 🎯 Objectives

- Analyze software metrics and defect patterns.
- Identify modules with higher defect counts.
- Investigate relationships between code complexity, code churn, test coverage, and defects.
- Apply data preprocessing and feature engineering techniques.
- Train and evaluate a machine learning model for defect-count prediction.
- Visualize findings and recommend software quality improvements.

## 📂 Dataset Description

The project uses five CSV files:

| File | Description |
|---|---|
| `modules.csv` | Module metadata, component, programming language, and size |
| `metrics.csv` | Code complexity, coupling, churn, and test coverage |
| `defects.csv` | Defect counts, severity, and release information |
| `commits.csv` | Commit count, contributor count, and changed lines |
| `releases.csv` | Release versions, dates, and module identifiers |

The synthetic dataset intentionally includes data-quality issues such as missing values, duplicate module-release records, inconsistent module names, an extreme complexity value, and an unmatched defect record.

## 🛠️ Technologies Used

- **Python** — Data analysis and model development
- **Pandas and NumPy** — Data processing and cleaning
- **Matplotlib and Seaborn** — Exploratory data analysis and visualization
- **Scikit-learn** — Machine learning and model evaluation
- **Google Colab** — Development environment
- **Microsoft Excel** — Data summaries and visualization

## ⚙️ Project Workflow

1. **Data Loading:** Import the five CSV datasets into Google Colab.
2. **Data Preprocessing:** Handle missing values, duplicate records, inconsistent module names, and extreme values.
3. **Data Integration:** Combine module, metric, defect, commit, and release information using module and release identifiers.
4. **Exploratory Data Analysis:** Visualize defect counts and investigate relationships between software metrics.
5. **Feature Engineering:** Select relevant input variables and the defect-count target.
6. **Machine Learning:** Train a Random Forest Regressor to predict defect counts.
7. **Model Evaluation:** Evaluate predictions using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R².
8. **Visualization and Recommendations:** Present important patterns and identify potential testing and code-review priorities.

## 📊 Visualizations

The project includes visualizations such as:

- Defects by module
- Code complexity versus defect count
- Code churn versus defect count
- Software metrics correlation heatmap
- Feature importance
- Actual versus predicted defect counts
- Test coverage comparisons

## 🤖 Machine Learning

**Algorithm:** Random Forest Regressor

**Target variable:** `defect_count`

**Input features:** Complexity, coupling, churn, test coverage, module size, commit count, contributors, and changed lines.

The model is evaluated on a held-out test set using MAE, RMSE, and R². The evaluation results are used to assess predictive performance and identify areas for improvement.

## 💡 Expected Outcomes

- Identify modules with relatively high defect counts.
- Explore software metrics associated with defect frequency.
- Understand the predictive usefulness of selected software metrics.
- Recommend code reviews and additional testing for modules that show recurring quality concerns.

## ⚠️ Limitations

- The dataset is synthetic and is intended for educational use.
- Observed relationships in the generated data should not be treated as evidence about real software systems.
- Model performance on synthetic data may not generalize to real-world software projects.
- Predictions should not be used for operational decisions without validation on representative real-world data.

## 🚀 How to Run

1. Clone or download this repository.
2. Open Google Colab.
3. Upload the five CSV files.
4. Open the project notebook.
5. Execute the notebook cells in sequence to reproduce the analysis and model evaluation.

## 👩‍💻 Project Purpose

This project demonstrates a complete data science workflow, from dataset preparation and exploratory analysis to machine learning, evaluation, visualization, and recommendations for software quality improvement.
