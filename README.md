# Netflix Data Cleaning and Analysis

## Project Overview

This project demonstrates an end-to-end data preparation and analysis workflow using the Netflix titles dataset. It combines Python, Pandas, Jupyter Notebook, and Microsoft SQL Server to perform data extraction, data-quality assessment, database loading, SQL-based data preparation, and analytical querying.

The objective is to identify data-quality issues, prepare the dataset for analysis, and answer business-oriented questions using SQL.

## Architecture and Workflow

The project follows this workflow:

1. **Data Source:** Netflix titles CSV dataset.
2. **Data Extraction and Inspection:** Python and Pandas are used to load, inspect, and profile the dataset.
3. **Data Quality Assessment:** Identify missing values, duplicate records, text-field issues, and data inconsistencies.
4. **Data Loading:** Load the dataset into Microsoft SQL Server for further processing.
5. **Data Preparation:** Use T-SQL to investigate data-quality issues and prepare data for analysis.
6. **SQL Analysis:** Run analytical queries to explore Netflix titles and derive business insights.

## Technology Stack

- **Python** — data extraction and preparation.
- **Pandas** — DataFrame operations and data-quality checks.
- **Jupyter Notebook** — interactive development and documentation.
- **Microsoft SQL Server** — relational data storage and analysis.
- **SQLAlchemy and pyodbc** — Python-to-SQL Server connectivity.
- **T-SQL** — data exploration, string manipulation, joins, aggregations, and analytical queries.

## Project Workflow

1. **Data Extraction:** Load the Netflix titles CSV dataset into a Pandas DataFrame.
2. **Data Inspection:** Examine dataset dimensions, sample records, columns, and values.
3. **Data Quality Assessment:** Investigate missing values, duplicate records, text-field lengths, and non-English characters.
4. **Database Integration:** Connect Python to SQL Server and load the dataset into a raw table.
5. **SQL Data Preparation:** Explore duplicates, split multi-value fields, examine date and duration fields, and investigate missing country information.
6. **Data Analysis:** Use SQL queries to explore genres, countries, directors, release years, and movie durations.

## Data Quality and Preparation

The project explores the following areas:

- Identifying missing values across columns.
- Examining the maximum length of text fields.
- Checking the preservation of non-English characters in Pandas.
- Investigating duplicate titles and records.
- Splitting comma-separated values, such as director names and genres, into separate records where required.
- Converting and examining date and duration fields.
- Investigating missing country information using related records.

## SQL Analysis

The analytical queries explore questions such as:

- How can duplicate Netflix records be identified?
- How are comedy titles distributed across countries?
- Which directors have the highest number of releases in a given year?
- What is the average duration of Netflix movies?
- Which directors are associated with both horror and comedy content?

The project applies SQL techniques including joins, aggregations, string manipulation, and analytical functions where required by the queries.

## Repository Contents

| File | Description |
|---|---|
| `Netflix Data Extract and Analysis.ipynb` | Python and Pandas data inspection, quality checks, and SQL Server integration. |
| `Netflix_Raw_Data.sql` | SQL script for creating the raw table and loading the Netflix dataset. |
| `Netflix_Data_Cleaning_Analysis.sql` | SQL queries for data preparation and analysis. |
| `README.md` | Project overview, technologies, workflow, and setup instructions. |

## Setup and Execution

### Prerequisites

- Python
- Jupyter Notebook
- Pandas, SQLAlchemy, and pyodbc
- Microsoft SQL Server
- An appropriate Microsoft ODBC Driver for SQL Server
- The Netflix titles CSV dataset

### Execution Steps

1. Obtain the Netflix titles CSV dataset from an authorized source.
2. Place the CSV file in the notebook's expected working directory, or update the file path in the notebook.
3. Create a SQL Server database named `NetflixDB`, or update the connection settings to use your database.
4. Verify the SQL Server instance, authentication method, and ODBC driver configuration.
5. Open `Netflix Data Extract and Analysis.ipynb` in Jupyter Notebook and execute the cells in order.
6. Review `Netflix_Raw_Data.sql` and execute the required raw-table setup or data-loading statements in the appropriate order.
7. Open `Netflix_Data_Cleaning_Analysis.sql` in SQL Server Management Studio (SSMS) and execute the statements in the appropriate order.

**Note:** The exact execution order may depend on the table creation and loading logic in the notebook and SQL scripts. Verify the scripts before running them in a new environment.

## Learning Outcomes

This project demonstrates practical experience with:

- Python and Pandas for data inspection and preparation.
- Relational database connectivity and data loading.
- SQL joins, aggregations, window functions, and string operations.
- Missing-value investigation and duplicate detection.
