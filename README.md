# Data Cleaning & Preprocessing with Python

A practical project focused on transforming raw, inconsistent data into a clean dataset ready for analysis and machine learning.

---

## Objective

Real-world data is messy. This project demonstrates how to systematically:

* Handle missing values
* Fix inconsistent formats
* Remove duplicates and outliers
* Prepare data for downstream tasks

---

## Workflow

```text
Raw Data → Exploration → Cleaning → Feature Processing → Final Dataset
```

---

## Project Structure

```text
Cleaning-Dataset-Using-python/
│
├── 01_Basic_Exploration/
├── 02_Numeric_Cleaning/
├── 03_Categorical_Cleaning/
├── 04_DateTime_Fixes/
├── 05_Advanced_Processing/
└── 06_Final_Output/
```

---

## Key Techniques

**Missing Values**

* Mean / Median (numeric)
* Mode (categorical)
* Forward / Backward fill (time-series)

**Data Cleaning**

* Duplicate removal
* Type correction
* Threshold-based column dropping

**Advanced Processing**

* Outlier detection (IQR, Z-score)
* Feature scaling (StandardScaler, MinMaxScaler)

---

## Example

```python
# Fill categorical missing values
data['embark_town'] = data['embark_town'].fillna(data['embark_town'].mode()[0])

# Drop columns with excessive missing values
df.dropna(thresh=len(df)*0.5, axis=1, inplace=True)
```

---

## Results

* Missing values handled
* Dataset cleaned and consistent
* Ready for machine learning pipelines

---

## Setup

```bash
git clone https://github.com/Tahir-Zaman-23DS14/Cleaning-Dataset-Using-python.git
cd Cleaning-Dataset-Using-python
pip install -r requirements.txt
```

---

## Author

Tahir Zaman
Data Science Student
