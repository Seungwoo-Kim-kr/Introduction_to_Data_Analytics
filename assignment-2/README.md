# Assignment 2 — Data exploration and preparation

Notebook: `ida_14588899.ipynb`

## What this notebook covers (based on the code)
This notebook focuses on:
- **A3 (initial exploration with tools)**:
  - Outlier detection on numeric attributes using boxplots and z-score
  - KMeans clustering on selected numeric features (with scaling)
  - PCA + visual exploration for clusters
  - Quick association check using grouped statistics (e.g., `poutcome` vs `Term Deposit`)
- **B. Data preprocessing (original data)**:
  - **B1**: `age` smoothing using:
    - Equi-width binning
    - Equi-depth binning
  - **B2**: `passed days` normalisation:
    - Min-max normalisation to [0,1]
    - Z-score normalisation
  - **B3**: Discretisation of `variation rate` into:
    - Low / Medium / High (and frequency counts)
  - **B4**: Binarisation of `contact` into {0,1}

The notebook also exports multiple Excel outputs for B1–B4 (see “Outputs” below).

## Input data
The notebook loads the student-specific dataset CSV (student ID filename).

Currently, the notebook uses an **absolute path** like:
`/Users/.../14588899.csv`

### Recommended setup
1. Create a local folder:
   - `assignment-2/data/`
2. Put your dataset file there:
   - `assignment-2/data/14588899.csv`
3. In the notebook, replace:
```python
file_path = "/Users/.../14588899.csv"