# E-commerce Data Cleaning Pipeline  
### *Client Simulation Project*

---

## Overview
Real-world e-commerce data is often inconsistent, incomplete, and difficult to use for analysis.  
This project simulates a client scenario where raw transactional data is cleaned, validated, and transformed into a structured, analysis-ready dataset.

---

## Data Transformation Preview

<p align="center">
  <img src="assets/images/before_data.png" width="45%" />
  <img src="assets/images/after_data.png" width="45%" />
</p>

<p align="center">
  <i>Before: Raw, inconsistent dataset &nbsp;&nbsp;|&nbsp;&nbsp; After: Clean, structured dataset</i>
</p>

---

## Objective
Develop a robust data cleaning pipeline to:
- Eliminate duplicate records  
- Standardize inconsistent data formats  
- Correct corrupted numerical values  
- Handle missing data effectively  
- Ensure schema consistency for downstream use  

---

## Dataset
**Source:** Brazilian E-commerce Dataset (Olist)  

**Tables Integrated:**
- Orders  
- Order Items  
- Payments  
- Customers  
- Products  

**Initial Dataset:**
- ~118,000 rows  
- ~30 columns  

---

## Data Challenges
To replicate real-world conditions, the dataset included:

- Duplicate records (~10% introduced)  
- Corrupted price values (strings, negatives, invalid entries)  
- Inconsistent categorical data (e.g., city names)  
- Mixed datetime formats  
- Missing values across product and delivery attributes  

---

## Cleaning Pipeline

### Data Preparation
- Merged multiple relational tables into a unified dataset  
- Preserved transaction-level granularity  

### Data Processing
- Removed duplicate records  
- Standardized text fields (lowercase, trimming)  
- Cleaned and validated numeric columns  
- Parsed inconsistent datetime formats  
- Handled missing values:
  - Imputed non-critical fields  
  - Removed critical null records  
- Enforced correct data types across all features  

---

## Results

| Metric             | Value            |
|--------------------|------------------|
| Final Rows         | ~112,000         |
| Columns            | 30               |
| Duplicates         | 0                |
| Missing Values     | Minimal          |

✔ Clean, structured, and reliable dataset  
✔ Ready for analytics, dashboards, and machine learning workflows  

---

## Tools & Technologies
- Python  
- Pandas  
- Jupyter Notebook  

---

## 📁 Project Structure

'''
ecommerce-data-cleaning/
├── assets/
│ ├── before_data.png
│ ├── after_data.png
│ └── pipeline.png # optional
│
├── data/
│ ├── raw_dirty_ecommerce_data.csv
│ └── cleaned_ecommerce_data.csv
│
├── notebooks/
│ └── data_cleaning_pipeline.ipynb
│
├── README.md
└── requirements.txt
'''

---

## Business Impact
This pipeline transforms unreliable raw data into a high-quality dataset that enables:
- Accurate business reporting  
- Consistent analytical outputs  
- Data-driven decision-making  

---

## Applications
- Freelance data cleaning services  
- Data preprocessing for machine learning  
- Preparing datasets for BI tools (Power BI, Tableau)  

---

## Author
**Harsh Rapaka**  
Data Science | Data Cleaning & Preprocessing