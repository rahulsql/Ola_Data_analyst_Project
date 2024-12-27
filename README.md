# Ola Data Analytics End-to-End Project

Welcome to the Ola Data Analytics End-to-End Project repository. This project demonstrates how to analyze a ride-sharing industry dataset using SQL, Excel, and Power BI. It is designed for data enthusiasts at all levels, from beginners to experienced professionals.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Setup and Prerequisites](#setup-and-prerequisites)
4. [Data Extraction with SQL](#data-extraction-with-sql)
5. [Data Analysis with Excel](#data-analysis-with-excel)
6. [Visualization with Power BI](#visualization-with-power-bi)
7. [Conclusion](#conclusion)

## Project Overview
This project explores a real-world scenario inspired by the ride-sharing industry. You'll learn how to:
- Query large datasets and prepare data using SQL.
- Perform in-depth analysis using Excel.
- Create dynamic dashboards using Power BI.

## Technologies Used
- **SQL:** For querying and preparing the data.
- **Microsoft Excel:** For data analysis and summarization.
- **Power BI:** For creating interactive dashboards and visualizations.

## Setup and Prerequisites
### Prerequisites
1. Install a SQL database management system (e.g., MySQL, PostgreSQL, or SQL Server).
2. Install Microsoft Excel (2016 or later preferred).
3. Install Power BI Desktop.

### Data
The dataset for this project is included in the `data` folder. It contains tables such as:
- `rides`: Information about individual rides.
- `drivers`: Data about drivers.
- `customers`: Customer demographics and behavior.

### Steps to Get Started
1. Clone this repository:
   ```bash
   git clone https://github.com/rahulsql/ola-data-analytics-project.git
   ```
2. Navigate to the project directory:
   ```bash
   cd ola-data-analytics-project
   ```
3. Import the dataset into your SQL database system.

## Data Extraction with SQL
In this phase, you will:
1. Write SQL queries to extract relevant data from the database.
2. Clean and preprocess the data for analysis.
3. Export the cleaned data to a CSV file for further analysis.

### Example Query
```sql
SELECT r.ride_id, r.date, d.driver_name, c.customer_name, r.fare_amount
FROM rides r
JOIN drivers d ON r.driver_id = d.driver_id
JOIN customers c ON r.customer_id = c.customer_id
WHERE r.date BETWEEN '2023-01-01' AND '2023-12-31';
```
Save the output as `cleaned_data.csv`.

## Data Analysis with Excel
1. Import the `cleaned_data.csv` file into Excel.
2. Perform the following tasks:
   - Use **Pivot Tables** to summarize rides by month.
   - Apply **Advanced Formulas** (e.g., `SUMIF`, `COUNTIF`) to calculate key metrics.
   - Create charts to visualize trends.

Save your Excel file as `data_analysis.xlsx`.

## Visualization with Power BI
1. Import `cleaned_data.csv` into Power BI.
2. Create a dashboard with:
   - A bar chart showing monthly ride counts.
   - A pie chart illustrating driver distribution.
   - A line graph for fare trends over time.
3. Publish the dashboard to Power BI Service (optional).

Save your Power BI project as `dashboard.pbix`.

## Conclusion
This project provides a complete pipeline for analyzing ride-sharing data. By following these steps, you will gain hands-on experience in:
- Extracting and transforming data with SQL.
- Conducting analysis and creating visualizations in Excel and Power BI.

Feel free to contribute or reach out if you have any questions!
