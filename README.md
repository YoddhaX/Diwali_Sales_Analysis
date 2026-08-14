# 🪔 Diwali Sales Analysis

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on Diwali sales data to understand customer purchasing behavior and identify important sales patterns.

The analysis uses **Python, Pandas, NumPy, Matplotlib, and Seaborn** to clean the data, explore customer demographics, analyze sales, and identify the categories and customer segments contributing most to sales.

---

## 🎯 Objectives

The main objectives of this project are:

* Analyze customer demographics
* Understand purchasing behavior based on gender and age
* Identify states with the highest number of orders
* Identify states generating the highest sales
* Analyze purchasing behavior based on marital status
* Analyze customers by occupation
* Identify popular product categories
* Find the most frequently ordered products
* Extract useful business insights from the sales data

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Jupyter Notebook** – Development environment

---

## 📂 Project Structure

```text
Diwali-Sales-Analysis/
│
├── Diwali_Sales_Analysis(1).ipynb
├── Diwali Sales Data.csv
└── README.md
```

---

## 🔄 Data Analysis Workflow

### 1. Import Libraries

The project starts by importing the required Python libraries:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

### 2. Load Dataset

The Diwali sales CSV file is loaded using Pandas:

```python
df = pd.read_csv('Diwali Sales Data.csv', encoding='unicode_escape')
```

### 3. Data Cleaning

The following preprocessing steps are performed:

* Checked dataset dimensions
* Inspected the first few records
* Checked column information
* Removed unnecessary columns such as `Status` and `unnamed1`
* Checked for missing values
* Removed rows containing null values
* Converted the `Amount` column into integer datatype

Example:

```python
df.drop(['Status', 'unnamed1'], axis=1, inplace=True)
df.dropna(inplace=True)
df['Amount'] = df['Amount'].astype('int')
```

---

# 📊 Exploratory Data Analysis

## 👨‍🦰 Gender Analysis

The project analyzes:

* Number of buyers by gender
* Total purchasing amount by gender

### Insight

The analysis shows that **female customers represent the larger buyer segment and have higher purchasing power than male customers** in this dataset.

---

## 🎂 Age Group Analysis

Customer purchasing behavior is analyzed across different age groups and genders.

### Insight

The **26–35 age group**, particularly females, represents an important customer segment in the dataset.

---

## 📍 State Analysis

The project analyzes the top states based on:

* Total number of orders
* Total sales amount

### Insight

The states contributing strongly to orders and sales include:

* **Uttar Pradesh**
* **Maharashtra**
* **Karnataka**

---

## 💍 Marital Status Analysis

Customer purchasing behavior is compared based on marital status and gender.

### Insight

The analysis indicates that **married women form a significant customer segment and show high purchasing power**.

---

## 💼 Occupation Analysis

The project analyzes customer distribution and sales across different occupations.

### Insight

Customers working in sectors such as:

* **IT**
* **Healthcare**
* **Aviation**

are among the important buyer segments in the dataset.

---

## 🛍️ Product Category Analysis

The project analyzes product categories based on:

* Number of products/orders
* Total sales amount

### Insight

The major product categories identified in the analysis include:

* **Food**
* **Clothing**
* **Electronics**

These categories account for a significant portion of the sales activity.

---

## 🏆 Top Products

The project also identifies the **top 10 products based on the total number of orders**.

This helps understand which individual products are most frequently purchased.

---

# 💡 Key Business Insights

Based on the analysis performed in the notebook:

1. **Female customers** are a major buyer segment.
2. Customers aged **26–35 years** are an important target group.
3. **Uttar Pradesh, Maharashtra, and Karnataka** are among the major states for orders and sales.
4. **Married women** show strong purchasing behavior.
5. Customers from **IT, Healthcare, and Aviation** occupations are important segments.
6. **Food, Clothing, and Electronics** are major product categories.
7. Product-level analysis can help identify the most frequently ordered products.

---

# 📈 Visualizations

The project uses several visualizations, including:

* Bar charts
* Gender distribution charts
* Age-group comparisons
* State-wise order analysis
* State-wise sales analysis
* Occupation analysis
* Product-category analysis
* Top-product analysis

These visualizations make it easier to identify patterns and trends in the sales data.

---

# 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project

```bash
cd Diwali-Sales-Analysis
```

### 3. Install required libraries

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open

```text
Diwali_Sales_Analysis(1).ipynb
```

Make sure `Diwali Sales Data.csv` is present in the same directory as the notebook.

---

# 📚 Skills Demonstrated

This project demonstrates practical knowledge of:

* Python
* Pandas DataFrames
* NumPy
* Data Cleaning
* Missing Value Handling
* Data Type Conversion
* `groupby()`
* Sorting and filtering
* Descriptive statistics
* Exploratory Data Analysis
* Data Visualization
* Matplotlib
* Seaborn
* Business Insight Generation

---
## 👨‍💻 Author

**Mayank Sahu**

Python | Data Analysis | Machine Learning | Web Development

---

## ⭐ If you found this project useful

Consider giving the repository a ⭐ on GitHub!
