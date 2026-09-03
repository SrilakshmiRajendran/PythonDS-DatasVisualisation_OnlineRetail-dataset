# Online Retail Data Analysis

## Project Overview

This project analyzes an Online Retail dataset to understand sales trends, customer behavior, and product performance.

The project involves data cleaning, feature engineering, exploratory data analysis, statistical analysis, data visualization, and business insight generation using Python.

## Objectives

- Clean and preprocess real-world retail data
- Handle missing values, duplicates, and invalid values
- Create new features for analysis
- Perform exploratory data analysis
- Analyze customer and product performance
- Visualize sales patterns using Matplotlib and Seaborn
- Derive meaningful business insights

## Dataset

**Online Retail Dataset – UCI Repository**

The dataset contains information such as:
- Invoice details
- Product/Stock Code
- Customer ID
- Quantity
- Unit Price
- Invoice Date
- Country

## Data Cleaning

The following data cleaning steps were performed:

- Removed records with missing `CustomerID`
- Removed duplicate records
- Removed negative `Quantity` values
- Removed invalid `UnitPrice` values (zero or negative)

## Feature Engineering

New features were created:

- `TotalPrice` = `Quantity × UnitPrice`
- `Year`
- `Month`
- `DayName`
- `Hour`
- `CustomerSegment`
- `OrderSize`
- `DayType`

## Data Analysis

The project uses:

- `describe()` for statistical overview
- `unique()` and `value_counts()` for categorical analysis
- `groupby()` and aggregation for:
  - Country-wise sales
  - Monthly sales
  - Product-wise sales
  - Customer-wise sales
- Sorting to identify top customers, countries, and products

## Statistical Analysis

The following statistical measures were calculated for `Quantity`, `UnitPrice`, and `TotalPrice`:

- Mean
- Median
- Mode
- Standard deviation
- Variance
- 25th, 50th, and 75th percentiles

## Data Visualization

The project includes visualizations using:

### Matplotlib
- Bar charts
- Histograms
- Box plots

### Seaborn
- Histogram with KDE

The visualizations were used to understand sales trends, customer purchasing behavior, and product sales distribution.

## Key Business Insights

- **Top Country:** The United Kingdom generated the highest total sales.
- **Best Sales Month:** November recorded the highest total sales.
- **Peak Sales Time:** 12 PM recorded the highest total sales.
- **Customer Behavior:** Most customers purchase relatively small quantities, while a few customers purchase significantly larger quantities.
- **High-Value Customers:** Most customers have relatively low total spending, while a small number of customers have significantly higher spending.
- **Top Products:** Most top products generate sales between 50,000 and 90,000, while a few products generate significantly higher sales.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Google Colab
- VS Code
- Git & GitHub

## Project Structure

```text
Online-Retail-Analysis/
│
├── data/
│   └── Online_Retail_Cleaned.csv
│
├── notebooks/
│   └── PythonDS_Datavisualisation_OnlineRetail_dataset.ipynb
│
├── README.md
│
└── requirements.txt
