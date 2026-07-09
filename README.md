#  Task 4 - Data Cleaning with Python

##  Objective

The objective of this project is to clean a deliberately messy e-commerce sales dataset and transform it into a clean, consistent, and analysis-ready dataset using Python.

---

##  Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Files

```
Task3_DataCleaning/
│
├── messy_ecommerce_sales_data.csv
├── Data_Cleaning.ipynb
├── cleaned_data.csv
└── README.md
```

---

##  Data Cleaning Tasks Performed

### 1. Data Quality Report
- Checked missing values in each column.
- Identified duplicate rows.
- Inspected data types.
- Detected inconsistent values and anomalies.

### 2. Missing Value Handling
- Filled missing values in **Category** using the mode.
- Filled missing values in **Quantity** using the median.
- Filled missing values in **Price** using the median.
- Calculated missing **Total** values using:
  ```
  Total = Quantity × Price
  ```

### 3. Duplicate Removal
- Identified duplicate records.
- Removed duplicate rows from the dataset.

### 4. Data Standardization
- Removed extra spaces from column names.
- Removed leading/trailing spaces from text values.
- Standardized categorical values.
- Converted date column into datetime format.

### 5. Outlier Detection
- Used the **Interquartile Range (IQR)** method to detect outliers.
- Applied capping to reduce the impact of extreme values while preserving valid records.

### 6. Data Type Correction
- Converted ID columns to string.
- Converted Quantity to integer.
- Converted Price and Total to float.
- Converted Order_Date to datetime.

### 7. Before vs After Comparison
Compared the dataset before and after cleaning based on:
- Row count
- Missing values
- Duplicate rows
- Data types

### 8. Export Cleaned Dataset
The cleaned dataset was saved as:

```
cleaned_data.csv
```

---

## Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## Outcome

The dataset is now:

- Clean
- Consistent
- Free from missing values
- Duplicate-free
- Properly standardized
- Correctly typed
- Ready for exploratory data analysis (EDA) and machine learning.

---

##  Author

**Simran Devi**  
B.Tech CSE Student  
Python | Data Analytics | Machine Learning