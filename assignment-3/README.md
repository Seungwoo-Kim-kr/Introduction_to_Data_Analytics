---

## 3) `assignment-3/README.md`

```md
# Assignment 3 — Data mining in action (Classification + Kaggle)

Notebook: `ida_a3_14588899.ipynb`

## Goal
Build classifiers to predict the target attribute **`subscribed`**:
- `0` = No
- `1` = Yes

Generate Kaggle-ready submission CSV files with the required column names:
- `row ID`
- `Prediction-subscribed`

## Datasets used (as referenced in the notebook)
The notebook references:
- `Assignment3-Marketing-Dataset.csv` (training/optimisation; includes target labels)
- `Assignment3-Unknown-Dataset.csv` (final prediction; no labels)
- Intermediate/preprocessed CSVs such as:
  - `Assignment3_Unknown_Preprocessed.csv`
  - `Assignment3_Train.csv`
  - `Assignment3_Train_Resampled.csv`
  - multiple preprocessing versions (`...Ver1`, `...Ver2`, `...Ver3`, `...Ver4`)

> The notebook currently uses absolute paths like `/Users/.../Desktop/UTS/...`.
> To run cleanly, switch these to relative paths (recommended below).

## Minimum required models (course spec)
At minimum, build one classifier for each:
- Decision Tree
- K-Nearest Neighbour (KNN)
- Random Forest
- Support Vector Machine (SVM)
- Neural Network (MLP)

## What this notebook implements (based on the code)
- Label encoding + scaling (StandardScaler / RobustScaler)
- Train/validation split (`train_test_split`)
- Parameter tuning using **GridSearchCV**
- Handling class imbalance using resampling techniques:
  - SMOTE
  - RandomOverSampler / RandomUnderSampler
- Model evaluation:
  - Accuracy, F1 score
  - Confusion matrix + classification report
- Kaggle submission file generation for multiple models:
  - `Kaggle_Submission_DT.csv`
  - `Kaggle_Submission_KNN.csv`
  - `Kaggle_Submission_RF.csv`
  - `Kaggle_Submission_SVM.csv`
  - `Kaggle_Submission_NN.csv`

## Recommended local folder layout
Inside `assignment-3/`: