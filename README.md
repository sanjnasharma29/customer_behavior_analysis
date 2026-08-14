# customer_behavior_analysis
# Data Analytics Project

## Overview

This project demonstrates an end-to-end **data analytics workflow**, from loading and exploring raw data to extracting insights through SQL and presenting findings in an interactive Power BI dashboard.

The project covers:

* Loading and analyzing a dataset using Python
* Exploratory Data Analysis (EDA)
* Data cleaning and preprocessing
* Running analytical queries using MySQL
* Creating an interactive Power BI dashboard
* Identifying trends, patterns, and business insights

## Dataset

The project uses a structured dataset containing business-related records for analysis.

The dataset is first loaded into Python for exploration and cleaning. After preprocessing, the cleaned data is imported into MySQL for SQL-based analysis and Power BI for visualization.

**Dataset:** Customer Shopping Behavior

**Key fields:** Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount, Location, Size, Color, Season, Review Rating, Subscription Status, Shipping Type, Discount Applied, Promo Code Used, Previous Purchase, Payment Method, Frequency of Purchases.

## Tools & Technologies

| Tool                     | Purpose                              |
| ------------------------ | ------------------------------------ |
| **Python**               | Data loading, EDA, and preprocessing |
| **Pandas**               | Data manipulation and cleaning       |
| **NumPy**                | Numerical operations                 |
| **Matplotlib / Seaborn** | Data visualization during EDA        |
| **MySQL**                | SQL-based data analysis              |
| **Power BI**             | Interactive dashboard and reporting  |
| **Jupyter Notebook**     | Python-based analysis                |

## Project Steps

### 1. Load Dataset

The dataset is imported into Python using Pandas and examined to understand its structure, columns, data types, and overall quality.

### 2. Exploratory Data Analysis

EDA is performed to identify:

* Dataset dimensions and structure
* Missing values
* Duplicate records
* Data types
* Outliers
* Distribution of important variables
* Trends and relationships between variables

### 3. Data Cleaning

The dataset is prepared for analysis by:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing inconsistent values
* Handling outliers where appropriate
* Creating or transforming required columns

### 4. SQL Analysis with MySQL

The cleaned dataset is loaded into MySQL, where SQL queries are used to answer analytical and business questions.

Examples include:

```sql
-- Example: Total sales
SELECT SUM(sales) AS total_sales
FROM sales_data;

-- Example: Sales by category
SELECT category, SUM(sales) AS total_sales
FROM sales_data
GROUP BY category
ORDER BY total_sales DESC;
```

The SQL analysis helps identify key trends, top-performing categories, regional performance, and other relevant business metrics.

### 5. Power BI Dashboard

The cleaned data and analytical results are used to build an interactive Power BI dashboard.

The dashboard includes relevant **KPIs, charts, filters, and visualizations** to make the analysis easy to understand and explore.

## Dashboard

The Power BI dashboard provides an interactive view of the major findings from the dataset.

**Key dashboard components may include:**

* Total Sales / Revenue
* Total Orders / Customers
* Category-wise performance
* Region-wise performance
* Monthly or yearly trends
* Top-performing products or categories
* Interactive slicers and filters

**Dashboard Preview:**
<img width="913" height="505" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/f4124f47-ce8a-4cd3-822b-312e67ba8d80" />

## Results & Key Insights

The analysis helps identify important patterns and trends within the dataset.

Key findings include:

* Identified overall business performance using key metrics.
* Determined the highest- and lowest-performing categories or segments.
* Analyzed trends over time.
* Compared performance across regions or other relevant dimensions.
* Used SQL queries to answer specific business questions.
* Presented the findings through an interactive Power BI dashboard.

> **Note:** Replace these points with the specific insights discovered in your project.

## Project Structure

```text
data-analytics-project/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── EDA_and_Cleaning.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── dashboard/
│   └── PowerBI_Dashboard.pbix
│
├── images/
│   └── dashboard.png
│
└── README.md
```

## How to Run

### 1. Clone the Repository

```bash
git clone <repository-url>
cd data-analytics-project
```

### 2. Install Python Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Run the Python Analysis

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook located in the `notebooks/` folder and run the cells to perform EDA and data cleaning.

### 4. Run MySQL Queries

1. Create a database in MySQL.
2. Import the cleaned dataset.
3. Open `sql/analysis_queries.sql`.
4. Execute the queries to reproduce the analysis.

### 5. Open the Power BI Dashboard

Open the `.pbix` file from the `dashboard/` folder using **Power BI Desktop**.

Update the data source if required and refresh the dashboard.

## Conclusion

This project demonstrates a complete **data analytics pipeline** using Python, MySQL, and Power BI. It combines data cleaning, exploratory analysis, SQL querying, and visualization to transform raw data into meaningful business insights.

## Skills Demonstrated

**Python | Pandas | EDA | Data Cleaning | SQL | MySQL | Data Visualization | Power BI | Business Analysis | Data Storytelling**
