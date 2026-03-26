       ### MINIProject 2 
       authors : Patrus Gurung an Juhi lee 

# Random Forest Classification — Imbalanced Dataset

## Overview
This project applies Random Forest classifiers to an imbalanced
binary classification dataset (42:1 class ratio) using various
techniques to handle class imbalance.

## Dataset
- 11,183 samples
- 6 continuous features (attr1–attr6)
- Binary target (class 0: 10,923 | class 1: 260)

## Tasks Covered
- (a) Exploratory data analysis and visualizations
- (b) Pipeline with ColumnTransformer and 5-fold CV
- (c) Hyperparameter tuning with GridSearchCV
- (d) Cross-validation strategy comparison
- (e) Weighted Random Forest
- (f) SMOTE and Random Undersampling
- (g) Evaluation metrics (Error Rate, F1, G-Mean)
- (h) Strengths and limitations discussion
- (i) Feature importance (MDI, Permutation, SHAP)

## Results Summary
| Model            | Error Rate | F1     | G-Mean |
|------------------|------------|--------|--------|
| Baseline RF      | 0.0139     | 0.8051 | 0.6927 |
| Tuned RF         | 0.0139     | 0.8051 | 0.6927 |
| Weighted RF      | 0.0139     | 0.8051 | 0.6927 |
| SMOTE RF         | 0.0165     | 0.8477 | 0.9137 |
| Undersampling RF | 0.0715     | 0.6733 | 0.9445 |

## Best Model
SMOTE RF — best balance across all three metrics

## How to Run
1. Clone the repository
   git clone https://github.com/YOUR_USERNAME/rf-classification-assignment.git

2. Install dependencies
   pip install -r requirements.txt

3. Open the notebook
   jupyter notebook notebooks/assignment.ipynb

## Requirements
See requirements.txt