# Customer Behavior Analysis

## Overview

This project focuses on analyzing customer purchasing behavior using a complete data analytics workflow. It includes data loading, cleaning, exploratory data analysis (EDA), SQL-based querying, and interactive dashboard creation using Power BI. The goal is to derive meaningful insights that can support business decision-making.

---

## Dataset

The dataset contains customer-related information such as:

* Customer ID
* Age, Gender
* Product details (item purchased, category, size, color)
* Purchase amount
* Location and season
* Review rating
* Subscription status
* Discount usage
* Payment method
* Purchase frequency

---

## Tools & Technologies

* **Python** (Pandas, NumPy, Matplotlib)
* **MySQL** (for database storage and querying)
* **SQLAlchemy & PyMySQL** (for Python–MySQL connection)
* **Power BI** (for dashboard creation)
* **Gamma** (for presentation)

---

## Steps Involved

### 1. Data Loading

* Imported dataset into Python using Pandas.
* Verified structure using `df.info()` and `df.head()`.

### 2. Data Cleaning

* Converted column names to lowercase.
* Replaced spaces with underscores.
* Renamed columns for consistency.
* Handled missing values (e.g., review ratings).
* Ensured correct data types.

### 3. Exploratory Data Analysis (EDA)

* Analyzed purchase patterns by gender, age, and category.
* Identified trends in customer spending.
* Checked distribution of ratings and purchase frequency.

### 4. Database Integration

* Created MySQL database: `customer_behavior`
* Connected using SQLAlchemy.
* Uploaded cleaned dataset into MySQL using:

  ```python
  df.to_sql("customer", engine, if_exists="replace", index=False)
  ```

### 5. SQL Analysis

Performed queries such as:

* Revenue by gender
* Customers spending above average
* Discount impact on purchases
* Purchase trends by category

### 6. Power BI Dashboard

* Connected Power BI to MySQL database.
* Built interactive dashboards including:

  * Revenue by gender
  * Category-wise sales
  * Purchase trends
  * Customer segmentation visuals

### 7. Reporting & Presentation

* Created a structured report summarizing findings.
* Designed a presentation using Gamma.

---

## Dashboard Highlights

* Revenue comparison (Male vs Female)
* Top-performing product categories
* High-value customers
* Discount vs purchase behavior
* Geographic purchase trends

---

## Results & Insights

* Identified key customer segments contributing to revenue.
* Observed patterns in discount usage and spending behavior.
* Highlighted top categories driving sales.
* Found trends in purchase frequency across demographics.

---

## How to Run

### Step 1: Install Dependencies

```bash
pip install pandas numpy matplotlib sqlalchemy pymysql
```

### Step 2: Run Python Script

* Load and clean dataset
* Export to MySQL

### Step 3: Setup MySQL

* Create database:

```sql
CREATE DATABASE customer_behavior;
```

### Step 4: Connect Power BI

* Server: `localhost:3306`
* Database: `customer_behavior`
* Authentication: Database (username & password)

### Step 5: Open Power BI File

* Open `.pbix` file
* Refresh data if needed

---

## Conclusion

This project demonstrates an end-to-end data analytics pipeline, combining Python, SQL, and Power BI to transform raw data into actionable insights. It showcases practical skills required for data analyst roles, including data cleaning, querying, visualization, and reporting.

---

