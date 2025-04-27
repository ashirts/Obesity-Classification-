# Obesity Classification Project

## Overview

This repository contains materials for a machine learning project analyzing and predicting obesity status using data from the UCI Machine Learning Repository.

The project includes:
- **obesity.csv** — The dataset used for analysis, containing lifestyle and demographic features.
- **Two Jupyter notebooks (.ipynb):**
  - **Obesity_Analysis_With_Weight.ipynb** — Analysis and model building with the weight feature included.
  - **Obesity_Analysis_Without_Weight.ipynb** — Analysis and model building with the weight feature excluded.
- **Write_Up/** — Final report materials, including:
  - The main written report in PDF format.
  - LaTeX files (.tex) used to compile the report.
  - Figures generated during the analysis and report creation.

## Project Summary

The goal of this project was to predict whether individuals are obese based on their demographics and lifestyle choices.
Both versions of the project — with and without the weight variable — train and evaluate a variety of machine learning models including:

- k-Nearest Neighbors (k-NN)
- Logistic Regression (with L1 and ElasticNet penalties)
- Linear Discriminant Analysis (LDA)
- Quadratic Discriminant Analysis (QDA)
- Decision Trees
- Random Forests
- Gradient Boosting
- Support Vector Machines (SVM)

Each model was tuned using **Optuna** for hyperparameter optimization and evaluated using **balanced accuracy** due to slight class imbalance. Feature importance was also explored using permutation methods to understand which factors most influenced model performance.

### Key Observations:
- Models generally performed better when **weight** was included as a feature.
- Even without the weight feature, models like **Gradient Boosting** maintained strong classification accuracy.
- Lifestyle and dietary habits (e.g., vegetable consumption, eating between meals) emerged as important predictors after removing weight.

## Technologies Used

- Python 3
- Jupyter Notebooks
- pandas, scikit-learn, matplotlib, seaborn
- Optuna (for hyperparameter tuning)
- LaTeX (for report generation)

## License

This project is for educational and academic purposes.

## Quick Start

To reproduce or explore the analysis:

```bash
# Clone the repository
git clone https://github.com/your-username/obesity-classification.git

# Open the Jupyter notebooks
jupyter notebook


