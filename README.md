# Bank-Loan-Portfolio-Analysis-SQL-Power-BI-
# Project Overview
This project analyses a bank loan portfolio to provide insights into lending performance, loan quality, borrower characteristics and portfolio trends.

The project was developed using Microsoft Power BI, with SQL Server used independently to validate the accuracy of key figures produced in Power BI. Key metrics from the Summary Dashboard were reproduced using SQL queries, and the SQL and Power BI results were compared to ensure that they returned consistent figures.

The analysis provides a structured view of the loan portfolio, helping stakeholders understand lending activity, assess loan quality, identify portfolio trends and explore borrower characteristics.

The project consists of three interactive Power BI dashboards:

### Dashboard 1 – Summary: Executive-level KPIs and loan portfolio performance

### Dashboard 2 – Overview: Trends, geographical distribution and borrower characteristics

### Dashboard 3 – Details: Detailed loan-level information

# Project Objective
The project aims to analyse a bank loan portfolio using SQL Server and Microsoft Power BI to assess lending performance, loan quality, borrower characteristics and portfolio trends, and present the findings through interactive dashboards that support informed decision-making.

The analysis focused on:

1. Measuring overall loan applications, funding and repayments
2. Assessing good and bad loan performance
3. Analysing loan performance across different loan statuses
4. Identifying lending trends over time
5. Examining the geographical distribution of lending activity
6. Understanding common loan terms and purposes
7. Analysing borrower characteristics such as employment length and home ownership
8. Providing detailed loan-level information for further investigation
9. Validating key Power BI figures independently using SQL Server

# Tools Used
Microsoft Power BI (Power Query, DAX)

Microsoft SQL Server

SQL Server Management Studio (SSMS)

# Data Preparation & Cleaning
## Data Connection
The required dataset was imported into Power BI from SQL Server.

SQL Server was also used independently to recreate selected calculations and validate key figures from the Power BI Summary Dashboard.

## Data Cleaning & Quality Checks
The dataset required little cleaning, but Power Query was used to review the dataset and confirm that the data was suitable for analysis.

The following Power Query features were used across the columns: Column Quality, Column Profile, Column Distribution.

These features were used to check for: Errors within columns, empty or missing values, unexpected or irregular data, data distribution and value patterns, general data consistency

The checks confirmed that the dataset was generally clean and suitable for analysis. 

This process helped ensure that the data used for calculations, modelling and visualisation was reliable and of good quality.

## Key Data Preparation Steps
1. Reviewed all columns for errors and empty values
2. Checked column quality and data distribution
3. Prepared date-related fields for analysis
4. Ensured the dataset was suitable for modelling and visualisation

# Data Modelling
A dedicated Calendar table was created in Power BI using DAX. The Calendar table includes: Date, Year, Month Name, Month Number. The Calendar table was connected to the loan data using the Issue Date field. This enabled consistent time-based analysis across the dashboards and allowed loan portfolio metrics to be analysed by year and month.

<img width="1313" height="559" alt="Data Model" src="https://github.com/user-attachments/assets/a1862bce-89fd-4e26-b66b-715d07fbe0f1" />

# DAX & Power BI Calculations
DAX was used to create calculated measures and support the analytical requirements of the dashboards.

Key DAX functionality demonstrated includes: SUM, CALCULATE, Filtering within measures, KPI calculations, Aggregations, Date-based calculations, Time intelligence. 

These calculations were used to generate the required loan portfolio metrics and support interactive dashboard analysis.

# SQL Data Validation
SQL was not used as the data source for the Power BI dashboards. Instead, SQL Server was used as an independent validation tool to verify the accuracy of key Power BI figures.

SQL queries were written to reproduce selected metrics from the Power BI Summary Dashboard.

The results generated in SQL were then compared with the corresponding Power BI figures to check that both approaches returned consistent results, which provided an additional layer of confidence in the accuracy of the reported figures.

SQL Functionalities Demonstrated: Database creation, Table creation, SELECT statements, WHERE filtering, GROUP BY, ORDER BY, COUNT, SUM, ROUND, Month and Year extraction, Data aggregation, Data validation and verification

# Dashboard 1 – Summary
The Summary Dashboard provides an executive-level overview of the bank's loan portfolio. It focuses on overall lending performance and loan quality, directly supporting the project's objective of assessing the health and performance of the portfolio.

<img width="1482" height="815" alt="Summary" src="https://github.com/user-attachments/assets/d4f9565b-9c84-4a7c-ae71-d0e4a850b501" />

## Key Performance Indicators
The dashboard includes: 

Total Loan Applications: Measures the total number of loan applications received during the selected period.

Total Funded Amount: Measures the total value of loans disbursed to borrowers.

Total Amount Received: Measures the total amount received from borrowers and provides an indication of repayment activity and cash flow.

Average Interest Rate: Measures the average interest rate across the loan portfolio.

Average Debt-to-Income Ratio (DTI): Measures the average DTI of borrowers and provides an indication of their overall financial position.

### Good Loan KPIs
The dashboard provides: Good Loan Application Percentage, Good Loan Applications, Good Loan Funded Amount, Good Loan Total Received Amount.
These metrics help assess the size and financial performance of loans classified as good.

### Bad Loan KPIs
The dashboard provides: Bad Loan Application Percentage, Bad Loan Applications, Bad Loan Funded Amount, Bad Loan Total Received Amount. These metrics provide visibility into the proportion and financial impact of loans classified as bad.

### Loan Status Grid
A detailed grid was created to analyse loan performance by Loan Status. The grid provides: Total Loan Applications, Total Funded Amount, Total Amount Received, Average Interest Rate, Average DTI. This allows users to compare the performance and characteristics of loans across different statuses.

### Dashboard 1  (Analysis Outcome)
The Summary Dashboard provides a clear view of the overall loan portfolio by showing the volume of applications, funding, repayments, interest rates and borrower DTI.

The Good and Bad Loan KPIs provide insight into loan quality and the financial contribution of different loan categories, while the Loan Status Grid allows users to compare portfolio performance across individual loan statuses.

These results directly support the project objective of assessing lending performance and overall loan portfolio health.

# Dashboard 2  - Overview 
The Overview Dashboard provides a broader analysis of lending trends, geographical activity and borrower characteristics.

<img width="1486" height="807" alt="Overview" src="https://github.com/user-attachments/assets/abe70550-c721-41ff-9c6b-8b0492648b00" />

### Monthly Lending Trends
A line chart displays lending activity by Issue Date. The visual helps identify: Monthly lending trends, changes in lending activity, potential seasonal patterns, long-term movements in lending activity. This helps stakeholders understand how lending performance changes over time.

### Geographical Analysis
A filled map visualises lending activity by state. The visual allows users to identify: States with significant lending activity, regional differences, geographical concentration of lending. This supports the analysis of where lending activity is concentrated across the portfolio.

### Loan Term Analysis
A donut chart shows the distribution of loans across different loan terms. This provides insight into borrower preferences for different repayment periods.

### Employment Length Analysis
A bar chart analyses lending metrics across different employment-length categories. This provides insight into lending activity among borrowers with different employment histories.

### Loan Purpose Analysis
A bar chart provides a breakdown of lending activity by loan purpose.

This helps identify the main reasons borrowers seek financing.

### Home Ownership Analysis
A treemap analyses lending activity across different home ownership categories.

This provides insight into borrower characteristics and the distribution of lending across home ownership groups.

### Metrics Analysed
The Overview Dashboard uses: Total Loan Applications, Total Funded Amount, Total Amount Received

### Dashboard 2 (Analysis Outcome)
The Overview Dashboard provides insight into how lending activity changes over time, where lending is concentrated geographically and the characteristics of borrowers within the portfolio.

The analysis of loan terms, employment length, loan purpose and home ownership provides a broader understanding of borrower behaviour and lending activity.

These findings directly support the project objective of understanding portfolio trends and borrower characteristics.

# Dashboard 3 – Details
The Details Dashboard provides a consolidated view of the underlying loan information.

Its primary objective is to provide users with a comprehensive and user-friendly interface for accessing detailed information about the loan portfolio, borrowers and loan performance.

The dashboard acts as a detailed reference point where users can examine individual records and gain a deeper understanding of the portfolio beyond the high-level KPIs.

### Dashboard 3 (Analysis Outcome)
The Details Dashboard supports further investigation by allowing users to move from high-level portfolio metrics to individual loan-level information.

<img width="1482" height="832" alt="Details" src="https://github.com/user-attachments/assets/099a1bee-088a-448b-bb7d-8ad22529dc3b" />

This complements the Summary and Overview dashboards and supports the overall objective by providing the detailed information needed to investigate specific loans and borrower records.

# Visualisation & Dashboard Development
Power BI was used to create and format a range of visual elements, including: KPI/Card visuals, line charts, bar charts, donut charts, filled maps, treemaps, tables and grid views. 

Additional dashboard functionality included: Interactive filtering, page navigation, Vvsual formatting, consistent dashboard layout, KPI presentation, time-based analysis, interactive reporting.

The dashboards were designed to provide both high-level portfolio monitoring and detailed analysis.

# Project Workflow
SQL Server → Power BI → Power Query Data Quality Checks → Data Preparation → Data Modelling → DAX Measures → Dashboard Development → SQL Validation → Business Insights

### Key Skills Demonstrated
**SQL Server:** Database Creation, Data Querying, Filtering, Data Aggregation, GROUP BY, ORDER BY, COUNT, SUM, ROUND, Month & Year Analysis, Data Validation, Data Accuracy Verification.

**Power BI:** SQL Server Data Connection, Power Query, Data Quality Checks, Data Transformation, Data Modelling, Relationship Creation, Date Table Development, DAX, CALCULATE, SUM, Time Intelligence, KPI Development, Data Visualisation, Dashboard Design, Interactive Reporting, Page Navigation. 

**Analytical Skills:** Financial Data Analysis, Loan Portfolio Analysis, KPI Analysis, Trend Analysis, Loan Quality Analysis, Borrower Analysis, Geographical Analysis, Data Validation, Data Quality, Business Intelligence, Insight Generation, Data-Driven Decision Making. 

# Project Outcome
The project achieved its objective of analysing a bank loan portfolio to assess lending performance, loan quality, borrower characteristics and portfolio trends.

The Summary Dashboard provides an executive-level view of portfolio performance and loan quality through KPIs, Good and Bad Loan analysis and Loan Status comparisons.

The Overview Dashboard provides insight into lending trends, geographical distribution and borrower characteristics, helping identify patterns across time, location, loan terms, employment length, loan purpose and home ownership.

The Details Dashboard provides access to individual loan-level information, allowing users to investigate the underlying records behind the portfolio-level analysis.

A key focus of the project was data accuracy and validation. Power Query was used to assess data quality before analysis, while SQL Server was independently used to reproduce and validate key Power BI figures. Comparing the SQL and Power BI results provided an additional layer of confidence in the accuracy of the reported metrics.

Overall, this project demonstrates the ability to take a financial dataset through the analytical process, from data quality checks and preparation to data modelling, DAX calculations, SQL validation, visualisation and interactive business reporting.















