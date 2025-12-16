# International-Debt-Analysis-Using-SQL-Data-Analytics

![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Project_Completed-28A745?style=for-the-badge&logo=checkmarx&logoColor=white)
![License](https://img.shields.io/badge/MIT_License-000000?style=for-the-badge&logo=open-source-initiative&logoColor=white)




This project analyzes **international debt statistics** across countries using **SQL and Python** to extract insights into global borrowing patterns.
The analysis focuses on identifying **high-debt countries**, **debt distribution trends**, and **key financial indicators** using structured queries and data analytics techniques.


## 📁 Dataset

* **Source:** International Debt Statistics (CSV format)
* **Data Stored In:** PostgreSQL
* **Table Name:** `international_debt`

### Table Schema

```sql
CREATE TABLE international_debt
(
  country_name VARCHAR(50),
  country_code VARCHAR(50),
  indicator_name TEXT,
  indicator_code TEXT,
  debt NUMERIC
);
```

### Data Import

```sql
\copy international_debt
FROM 'international_debt.csv'
DELIMITER ','
CSV HEADER;
```


<br>


## 🛠️ Tech Stack

* **Python**
* **PostgreSQL**
* **SQL**
* **Pandas**
* **Jupyter Notebook**

<br>

## 🔍 Project Objectives

* Store structured financial data using SQL
* Analyze international debt across countries and indicators
* Identify countries with the highest total debt
* Understand debt distribution across economic indicators
* Perform aggregation and ranking using SQL queries
* Combine SQL with Python for analysis and reporting

<br>

## 📊 Analysis Performed

### ✔️ Database & SQL Analysis

* Created relational table schema for international debt data
* Imported large CSV data into PostgreSQL
* Used SQL queries with:

  * `SUM`, `AVG`, `MAX`
  * `GROUP BY`, `ORDER BY`
  * Filtering by country and indicators
* Ranked countries based on total debt
* Analyzed debt contribution by indicator type

<br>

## 📈 Key Insights

* Identified countries with the highest accumulated debt
* Highlighted indicators contributing most to global debt
* Observed significant variation in debt distribution across regions
* Demonstrated how SQL can be effectively used for financial analysis at scale

<br>

## 🚀 How to Run the Project

1. Create the PostgreSQL table using the provided SQL script
2. Import the CSV file into the database
3. Open the Jupyter Notebook
4. Run SQL queries and analysis cells

<br>

## 🏁 Conclusion

This project showcases the practical application of SQL and Python for analyzing global financial datasets.
The insights derived can help understand international borrowing patterns and demonstrate how structured data analytics supports informed financial decision-making.
