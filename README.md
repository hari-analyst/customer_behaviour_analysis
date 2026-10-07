
📊 Data Analytics Project

Overview

This project demonstrates an end-to-end data analytics workflow, starting from raw data loading and exploration to SQL-based analysis, interactive Power BI visualization, reporting, and presentation.

The objective is to transform raw business data into meaningful insights that can support data-driven decision-making.

Project Workflow

Dataset → Python EDA → Data Cleaning → SQL Server Analysis → Power BI Dashboard → Report → Presentation



📁 Dataset

The project uses a structured dataset containing business-related records for analysis.

The dataset was initially loaded and explored using Python to understand:

- Dataset structure and dimensions
- Data types
- Missing values
- Duplicate records
- Outliers
- Categorical and numerical variables
- Key business metrics and trends



🛠️ Tools & Technologies


Python -- Data loading, EDA, and data cleaning
Pandas -- Data manipulation and preprocessing
NumPy -- Numerical analysis
Matplotlib / Seaborn -- Exploratory data visualization
SQL Server -- Data querying and business analysis
Power BI -- Interactive dashboard development
Gamma --  Presentation creation
Microsoft Excel -- Data inspection/supporting analysis

---

🔄 Project Steps

1. Data Loading

The dataset was imported into Python using Pandas.

import pandas as pd

df = pd.read_csv("data/dataset.csv")

print(df.head())
print(df.shape)
print(df.info())

The initial inspection helped identify the dataset's structure, columns, data types, and potential quality issues.

---

2. Exploratory Data Analysis (EDA)

EDA was performed to understand the data and identify important patterns.

Key activities included:

- Checking dataset dimensions
- Analysing numerical and categorical columns
- Identifying missing values
- Detecting duplicate records
- Analysing distributions
- Identifying outliers
- Studying relationships between variables
- Creating exploratory visualizations

Example:

df.describe()
df.isnull().sum()
df.duplicated().sum()

---

3. Data Cleaning

The raw dataset was cleaned and prepared for analysis.

 cleaning activities included:

- Handling missing values
- Removing duplicate records
- Correcting data types
- Standardizing column values
- Handling inconsistent entries
- Formatting dates
- Validating numerical values

The cleaned dataset was then prepared for SQL Server and Power BI analysis.

---

4. SQL Server Analysis

The cleaned data was loaded into SQL Server for structured business analysis.

SQL queries were used to answer important business questions such as:

- What are the overall sales/revenue trends?
- Which products or categories perform best?
- Which regions or segments contribute the most?
- What are the monthly/quarterly trends?
- Which customers or products require attention?

Example:

SELECT
    Category,
    SUM(Sales) AS Total_Sales
FROM Sales_Data
GROUP BY Category
ORDER BY Total_Sales DESC;

SQL was primarily used to perform aggregation, filtering, grouping, ranking, and trend analysis.

---

5. Power BI Dashboard

The analysed data was connected to Power BI to create an interactive dashboard.

Dashboard Components

The dashboard includes:

- KPI cards
- Sales/revenue overview
- Category analysis
- Regional analysis
- Time-based trends
- Top-performing products/customers
- Interactive filters and slicers

The dashboard was designed to provide a quick overview of business performance while allowing users to explore specific areas interactively.

---

📊 Dashboard

Power BI Dashboard Preview





The dashboard enables users to filter and analyse the data based on relevant dimensions such as date, category, region, product, or customer segment.

---

📈 Key Results & Insights

The analysis generated several business insights from the dataset.

Key Findings

- Identified the highest-performing products/categories.
- Analysed regional/segment-wise performance.
- Identified important sales/revenue trends over time.
- Compared high-performing and low-performing business segments.
- Identified areas that may require further investigation or improvement.

Business Impact

The analysis converts raw transactional data into actionable information that can help stakeholders:

- Monitor business performance
- Identify growth opportunities
- Understand customer/product behaviour
- Detect underperforming segments
- Support data-driven decision-making

«Replace these generic findings with your actual numbers and insights. Recruiters care much more about specific results than statements like "identified valuable insights."»

---

📄 Project Report

A detailed project report was created covering:

1. Business problem
2. Dataset description
3. Data preprocessing
4. Exploratory data analysis
5. SQL analysis
6. Power BI dashboard
7. Key findings
8. Business recommendations
9. Conclusion

---

🎯 Presentation

A project presentation was created using Gamma to communicate the analysis and findings in a concise, business-friendly format.

The presentation covers:

- Problem statement
- Analytical approach
- Dataset
- Key insights
- Dashboard
- Business recommendations
- Conclusion

---

▶️ How to Run

Prerequisites

Install the required Python libraries:

pip install pandas numpy matplotlib seaborn

Step 1 — Clone the Repository

git clone <repository-url>
cd <project-folder>

Step 2 — Load the Dataset

Place the dataset inside:

data/

Step 3 — Run Python Analysis

Open the Jupyter Notebook:

notebooks/EDA.ipynb

Run the notebook to perform data loading, EDA, and data cleaning.

Step 4 — SQL Server

1. Open SQL Server Management Studio.
2. Create the required database.
3. Import the cleaned dataset.
4. Execute the SQL scripts available in:

sql/

Step 5 — Power BI

Open the Power BI file:

powerbi/<customer_shopping_behaviour>.pbix

Update the SQL Server connection if required and refresh the dataset.


📂 Project Structure

Data-Analytics-Project/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   └── EDA.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── dashboard.pbix
│
├── report/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
├── images/
│   └── dashboard.png
│
└── README.md

💡 Skills Demonstrated

- Data Cleaning & Preprocessing
- Exploratory Data Analysis
- Python & Pandas
- SQL Server
- SQL Querying
- Data Visualization
- Power BI Dashboard Development
- Business Analysis
- Data Storytelling
- Report Writing
- Presentation Development


⭐ Conclusion

This project demonstrates an end-to-end approach to solving a data analytics problem — from raw data preparation and exploratory analysis to SQL-based investigation, interactive dashboard development, and business-focused communication of insights.
