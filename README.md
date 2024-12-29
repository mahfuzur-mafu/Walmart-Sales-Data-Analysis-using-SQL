# Walmart Sales Data Analysis using SQL
 

## Overview
This project provides an end-to-end data analysis solution for Walmart sales data. Using Python and SQL, it extracts critical business insights by solving key analytical problems. This repository is ideal for data analysts aiming to enhance their skills in data manipulation, SQL querying, and exploratory data analysis.

---

## Table of Contents
- [Overview](#overview)
- [Project Workflow](#project-workflow)
- [Key Features](#key-features)
- [Requirements](#requirements)
- [Usage Instructions](#usage-instructions)
- [Dataset](#dataset)
- [SQL Queries](#sql-queries)
- [Results and Insights](#results-and-insights)

---

## Project Workflow
1. **Data Acquisition**
   - Download Walmart sales data using the Kaggle API.
   - Place the dataset in the `data/` directory for processing.

2. **Data Preparation**
   - Load raw data into a Pandas DataFrame for exploration.
   - Clean and preprocess the data by:
     - Removing duplicates.
     - Handling missing values.
     - Formatting currency and ensuring consistent data types.

3. **Feature Engineering**
   - Add calculated fields like total transaction amount (`unit_price * quantity`) for streamlined SQL analysis.

4. **Data Loading**
   - Load the cleaned data into MySQL and PostgreSQL databases using Python's `sqlalchemy`.

5. **SQL Querying**
   - Perform complex analyses to solve business problems, including:
     - Revenue trends by branch and category.
     - Identifying high- and low-performing products and branches.
     - Analyzing peak sales times and preferred payment methods.

6. **Visualization and Reporting**
   - Optionally, use visualization tools (e.g., Matplotlib or Tableau) to present findings.

---

## Key Features
- **Comprehensive Data Cleaning:** Ensures high data quality by handling missing values, duplicates, and inconsistent formats.
- **SQL-Powered Analysis:** Includes advanced queries to extract actionable insights.
- **Database Integration:** Utilizes MySQL and PostgreSQL for data storage and querying.
- **Automated Workflow:** Python scripts automate data processing and database operations.

---

## Requirements
- **Python 3.8+**
- Libraries:
  - pandas
  - numpy
  - sqlalchemy
  - mysql-connector-python
  - psycopg2
- SQL Databases:
  - MySQL
  - PostgreSQL
- Kaggle API Key (for dataset download)

---

## Usage Instructions
1. **Clone the Repository**
   ```bash
   git clone <repo-url>
   cd <repo-directory>



## Dataset Description
This project uses transactional data from Walmart to derive insights into sales, profitability, and customer behavior. The dataset includes the following key columns:

- **branch**: Identifier for branches
- **city**: Location of branches
- **payment_method**: Mode of payment
- **unit_price**: Price per unit
- **quantity**: Number of units sold
- **rating**: Customer ratings
- **profit_margin**: Profit margin on products
- **date**: Transaction date
- **time**: Transaction time
- **category**: Product category
- **total**: Total transaction amount

## Analysis

### Basic Queries
- **Fetch all data**
- **Count total transactions**

### Grouping and Aggregation
- **Count distinct payment methods and transactions per method**
- **Calculate the total quantity sold by payment method**

### Branch and Category Analysis
- **Identify low-performing branches**
- **Find the highest-rated categories per branch**
- **Determine low-performing categories**

### Shift and Time-based Analysis
- **Analyze busiest day per branch**
- **Categorize sales into Morning, Afternoon, and Evening shifts**

### Revenue Comparison
- **Compare branch revenues for 2022 and 2023, highlighting revenue declines**

## Results and Insights
Key insights derived from the project include:

- **Sales Insights**: Identification of key product categories, branches with the highest sales, and preferred payment methods.
- **Profitability**: Insights into the most profitable product categories and branch locations.
- **Customer Behavior**: Trends in customer ratings, payment preferences, and peak shopping hours.
- **Branch Comparisons**: Revenue trends and performance evaluations over time, including a comparison of branch revenues for 2022 and 2023.

## Conclusion
This analysis provides valuable insights into Walmart's transactional data, helping to understand sales performance, customer preferences, and profitability across different branches and product categories. These insights can inform strategic decisions to enhance overall business performance.
