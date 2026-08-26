# Bank-Loan-Portfolio-Analysis-SQL-Power-BI-
This project analyses a bank loan portfolio to provide insights into lending performance, loan quality, borrower characteristics and portfolio trends.

The project was developed using Microsoft Power BI, with SQL Server used independently to validate the accuracy of key figures produced in Power BI. Key metrics from Dashboard 1 were reproduced using SQL queries, and the SQL and Power BI results were compared to ensure they returned the same figures.

The analysis was designed to help stakeholders monitor the health of the loan portfolio, understand lending trends and assess the performance of different loan categories.

The project consists of three interactive Power BI dashboards:

### Dashboard 1 – Summary: Executive-level KPIs and loan portfolio performance

### Dashboard 2 – Overview: Trends, geographical distribution and borrower characteristics

### Dashboard 3 – Details: Detailed loan-level information

# Business Objectives
The analysis aims to answer key questions around:

How many loan applications has the bank received?
How much has the bank funded?
How much has been received from borrowers?
What is the average interest rate?
What is the average borrower Debt-to-Income Ratio (DTI)?
What proportion of the portfolio consists of good and bad loans?
How does lending performance change over time?
Which states generate the highest lending activity?
What are the most common loan terms and purposes?
How do employment length and home ownership relate to lending activity?
What does the overall loan portfolio look like at a detailed level?

# SQL Data Validation
SQL was not used as the data source for the Power BI dashboards. Instead, SQL was used as an independent validation tool to verify the accuracy of the analysis.

A new SQL database and table were created, and SQL queries were written to reproduce key metrics from the Power BI Summary Dashboard.

The results generated in SQL were compared against the corresponding Power BI figures, with the objective of ensuring that both approaches returned consistent results.

### SQL functionalities demonstrated: 
Database creation, Table creation, SELECT statements, WHERE filtering, GROUP BY, ORDER BY, COUNT, SUM, ROUND, Month and Year extraction, Data aggregation, Data validation and verification.

# Power BI Data Preparation & Modelling
### Data Connection
The required dataset was imported into Power BI from SQL Server.

### Data Cleaning
Power Query was used to prepare the dataset for analysis.

### Key transformations included:
Cleaning the dataset
Preparing date-related fields for analysis
Ensuring data was suitable for modelling and visualisation

### Data Modelling
A dedicated Calendar/Date table was created in Power BI using DAX time-intelligence functionality.
The Calendar table includes: Date, Year, Month Name, Month Number.

The Calendar table was then connected to the loan data using the Issue Date field.

This enabled consistent time-based analysis across the dashboards and allowed metrics to be analysed by year and month.

### Power BI functionalities demonstrated: 
DAX was used to create calculated measures and support the dashboard's analytical requirements.

Key DAX functionality demonstrated includes: SUM, CALCULATE. Filtering within measures, KPI calculations, Time intelligence, Date-based calculations, Aggregations.
These calculations were used to generate the required loan portfolio metrics and support interactive dashboard analysis.


# Dashboard 1 (Summary)
The Summary Dashboard provides an executive-level overview of the bank's loan portfolio.

### Key Performance Indicators

The dashboard includes: 

Total Loan Applications: Measures the total number of loan applications received during the selected period.

Total Funded Amount: Measures the total value of loans disbursed to borrowers.

Total Amount Received: Measures the total amount received from borrowers, providing an indication of loan repayment and cash flow.

Average Interest Rate: Measures the average interest rate across the loan portfolio.

Average Debt-to-Income Ratio (DTI): Measures the average DTI of borrowers to provide an indication of their financial position.

### Good Loan KPIs

The dashboard provides the following Good Loan metrics: Good Loan Application Percentage, Good Loan Applications, Good Loan Funded Amount and Good Loan Total Received Amount.

These metrics help assess the size and financial performance of loans classified as good.

### Bad Loan KPIs

The dashboard provides: Bad Loan Application Percentage, Bad Loan Applications, Bad Loan Funded Amount and Bad Loan Total Received Amount

These metrics provide visibility into the proportion and financial impact of loans classified as bad.

### Loan Status Grid

A detailed grid view was created to analyse loan performance by Loan Status.

The grid provides: Total Loan Applications, Total Funded Amount, Total Amount Received, Average Interest Rate and Average DTI

This allows users to compare the performance and characteristics of loans across different statuses.

# Dashboard 2 (Overview)

The Overview Dashboard provides a broader view of lending trends, geographical activity and borrower characteristics.

### Monthly Lending Trends

A Line Chart displays lending activity by Issue Date to identify: Monthly trends, Changes in lending activity, Potential seasonal patterns, Long-term lending movements and Regional Analysis.

A Filled Map visualises lending activity by state, allowing users to identify: States with significant lending activity, Regional differences, Geographic concentration of lending, Loan Term Analysis

A Donut Chart shows the distribution of loans across different loan terms. The visual helps stakeholders understand borrower preferences for different repayment periods.

Employee Length Analysis: A Bar Chart analyses lending metrics across different employment lengths. This provides insight into the relationship between employment history and lending activity.

Loan Purpose Analysis: A Bar Chart provides a breakdown of lending activity by loan purpose. This helps identify the main reasons borrowers seek financing.

Home Ownership Analysis: A Treemap analyses lending activity based on home ownership categories. This provides a hierarchical view of the relationship between home ownership and loan activity.

### Metrics Analysed
The Overview Dashboard uses: Total Loan Applications, Total Funded Amount, Total Amount Received

# Dashboard 3 (Details)

The Details Dashboard provides a consolidated view of the underlying loan information. Its primary objective is to provide users with a comprehensive and user-friendly interface for accessing detailed information about the loan portfolio, borrowers and loan performance. The dashboard acts as a detailed reference point where users can examine individual records and gain a deeper understanding of the portfolio beyond the high-level KPIs.

# Visualisation & Dashboard Development

Power BI was used to create and format a range of visual elements, including: KPI/Card visuals. Line charts, Bar charts, Donut charts, Filled maps. Treemaps, Tables/Grid views.

Additional dashboard functionality included: Interactive filtering, Page navigation, Visual formatting, Consistent dashboard layout, KPI presentation, Time-based analysis

# Key Skills Demonstrated
### SQL
Database Creation, Table Creation, Data Querying, Filtering, Aggregation, GROUP BY, ORDER BY, COUNT, SUM, ROUND, Month & Year Analysis
Data Validation, Data Accuracy Verification
### Power BI
SQL Server Data Connection, Power Query, Data Cleaning, Data Transformation, Data Modelling, Relationship Creation, Calendar/Date Table Development, DAX, CALCULATE, SUM, Time Intelligence, KPI Development, Data Visualisation, Dashboard Design, Interactive Reporting, Page Navigation
### Analytical Skills
Financial Data Analysis, Loan Portfolio Analysis, KPI Analysis, Trend Analysis, Data Validation, Data Quality, Business Intelligence, Data-Driven Decision Making, Insight Generation.

# Project Outcome

This project demonstrates the ability to take a business-focused lending dataset through the complete analytical process, from data preparation and validation to modelling, KPI development and interactive reporting.

A key focus of the project was data accuracy. SQL was used independently to reproduce and validate key Power BI figures, providing an additional layer of confidence in the reported results.

The resulting dashboards provide stakeholders with a structured view of loan applications, funding, repayments, loan quality, borrower characteristics, geographical trends and loan performance, supporting more informed analysis and decision-making.





