# ❤️ Heart Disease Data Analysis (EDA)

An Exploratory Data Analysis (EDA) project using Python to examine heart disease data, clean duplicate records, explore medical attributes, and visualize patterns in the dataset.

**Repository:** [Heart-Disease-Prediction](https://github.com/kk7776646-coder/Heart-Disease-Prediction)  
**Notebook:** [`heartDisease.ipynb`](heartDisease.ipynb)

## 📌 Project Overview

This project explores a heart disease dataset using Python's data analysis and visualization libraries. The notebook loads the data, checks its structure and quality, identifies missing values and duplicate records, removes duplicate rows, and uses visualizations to explore relationships between patient attributes and the target label.

The project is focused on **data cleaning and exploratory data analysis**. It does not implement or evaluate a machine learning prediction model.

## 🎯 Objectives

- Inspect the dataset structure and data types.
- Check for missing values and duplicate records.
- Remove duplicate rows before further analysis.
- Explore numerical and categorical medical features.
- Visualize distributions and relationships between features and the target.
- Practice data analysis with Pandas, NumPy, Matplotlib, and Seaborn.

## 📊 Dataset

The notebook loads a CSV file named `heart.csv`. The dataset needs to be obtained separately; it is not currently included in this repository.

- **Source:** Kaggle dataset (the exact dataset URL is not recorded in the notebook)
- **File expected by the notebook:** `heart.csv`
- **Initial shape:** 1,025 rows × 14 columns
- **After duplicate removal:** 302 rows × 14 columns
- **Missing values:** The notebook's missing-value check reports zero missing values in each column
- **Duplicate rows detected:** 723

> **Data note:** Duplicate removal reduces the data from 1,025 to 302 rows. This is a substantial change, so the dataset's origin and the meaning of these repeated rows should be checked before drawing conclusions. Duplicate rows are not always erroneous in every dataset.

### Dataset Features

The notebook uses the following 14 columns:

| Column | Description |
|---|---|
| `age` | Patient age |
| `sex` | Sex category, encoded numerically |
| `cp` | Chest pain type, encoded numerically |
| `trestbps` | Resting blood pressure |
| `chol` | Serum cholesterol |
| `fbs` | Fasting blood sugar indicator |
| `restecg` | Resting electrocardiogram category |
| `thalach` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina indicator |
| `oldpeak` | ST depression associated with exercise |
| `slope` | Slope of the peak exercise ST segment |
| `ca` | Number of major vessels, encoded numerically |
| `thal` | Thal-related category, encoded numerically |
| `target` | Heart disease target label |

The exact meanings of encoded categories should be checked against the documentation for the specific Kaggle dataset.

## 🛠️ Tools and Libraries

- **Python** — Core programming language
- **Jupyter Notebook** — Interactive analysis
- **Pandas** — Loading, inspecting, and manipulating tabular data
- **NumPy** — Numerical operations
- **Matplotlib** — Plotting and chart formatting
- **Seaborn** — Statistical visualizations

## 🔍 Analysis Workflow

### 1. Import Libraries and Load Data

The notebook imports Pandas, NumPy, Matplotlib, and Seaborn, then loads `heart.csv` into a Pandas DataFrame.

### 2. Inspect the Dataset

- Preview the first and last rows.
- Check the shape and column names.
- Review column data types and non-null counts.
- Generate descriptive statistics.

### 3. Check Data Quality

- Count missing values in each column.
- Identify duplicate rows.
- Remove duplicate rows using Pandas.
- Recheck the dataset shape after duplicate removal.

### 4. Exploratory Data Analysis

The notebook explores the distributions of patient attributes and compares selected categorical features with the `target` label.

### 5. Visualize Relationships

Charts are used to inspect numerical correlations and compare categories across the dataset.

## 📈 Visualizations in the Notebook

The notebook includes visualizations such as:

- **Correlation heatmap** — Displays pairwise correlations between numerical columns.
- **Age distribution** — Uses a histogram with a KDE curve to inspect the age distribution.
- **Sex distribution** — Compares the counts of the encoded sex categories.
- **Sex vs. target** — Compares target categories across sex groups.
- **Chest pain type distribution** — Shows counts for the encoded chest pain categories.
- **Chest pain vs. target** — Compares target categories across chest pain groups.
- **Fasting blood sugar vs. target** — Explores the distribution of the target across fasting blood sugar categories.

These charts describe patterns in this dataset; they do not establish cause-and-effect relationships.

## 💡 Findings from the Notebook

The following data-quality results are visible in the notebook:

- The initial dataset contains 1,025 rows and 14 columns.
- The missing-value check reports zero missing values in every column.
- The notebook detects 723 duplicate rows.
- After `drop_duplicates()`, the dataset contains 302 rows and 14 columns.

The notebook also generates a correlation heatmap and several distribution and category-comparison plots. Specific medical conclusions are not stated here; interpret them only after reviewing the charts and verifying the dataset's category definitions.

## 🚀 Setup and Run

### Prerequisites

Install Python and Jupyter Notebook, or use Anaconda.

### 1. Clone the repository

```bash
git clone https://github.com/kk7776646-coder/Heart-Disease-Prediction.git
cd Heart-Disease-Prediction
```

### 2. Install the libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Obtain the dataset

Obtain the appropriate Kaggle dataset and place the CSV file named `heart.csv` in the working directory used by the notebook. The notebook currently loads the file with:

```python
data = pd.read_csv("heart.csv")
```

If the CSV is stored in another directory, update the path accordingly.

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `heartDisease.ipynb` and run the cells in order.

## 📁 Project Structure

```text
Heart-Disease-Prediction/
├── README.md
└── heartDisease.ipynb
```

The dataset file `heart.csv` is required to run the notebook but is not currently included in the repository.

## ⚠️ Limitations

- The exact Kaggle dataset URL and its full documentation are not recorded in the notebook.
- Removing 723 duplicate rows substantially changes the dataset; the cause and appropriateness of this step should be verified.
- Encoded category values should be interpreted using the source dataset's documentation.
- Correlation does not imply causation.
- Exploratory data analysis alone does not diagnose heart disease or establish individual medical risk.
- This repository does not claim a trained model, prediction accuracy, or clinical validation.

## 🩺 Medical Disclaimer

This project is for educational and data analysis purposes only. It is **not a medical diagnostic tool** and must not be used to diagnose, treat, or make clinical decisions. Consult a qualified healthcare professional for medical advice.

## 👨‍💻 Author

**Kalamuddin Khan**

- GitHub: [@kk7776646-coder](https://github.com/kk7776646-coder)
- Project: [Heart-Disease-Prediction](https://github.com/kk7776646-coder/Heart-Disease-Prediction)

---

If you find this project useful, consider starring the repository.
