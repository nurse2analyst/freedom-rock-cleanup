Freedom Rock Bicycles: Employee & Order Data Cleanup (Excel Project)
Project Overview

This project focused on cleaning and standardizing employee and order data for Freedom Rock Bicycles. The data had been inconsistently managed, leading to formatting issues, missing values, and lack of standardization. My objective was to make the dataset accurate, consistent, and ready for reporting and analysis.

The work was completed in two main areas:

Employees worksheet — standardizing staff records, correcting errors, and creating calculated fields.

Orders worksheet — parsing raw order data, reformatting for clarity, and preparing it for quality checks.

📂 Example files:

Raw Data

Cleaned Data

Work Completed
Employees Worksheet

Removed duplicate entries.

Standardized formatting (state abbreviations, phone numbers, bonus percentages).

Cleaned text using TRIM() and corrected spelling errors.

Reorganized columns for better readability.

Updated job titles (“Salesman” → “Salesperson”).

Added calculated fields:

Years of service → =YEAR(TODAY()) - YEAR(Hire Date)

Salary with Bonus → =Salary * (1 + Bonus %)

Orders Worksheet

Converted comma-separated data into columns.

Reformatted Order Date values and standardized headers.

Split full employee names into First Name / Last Name.

Adjusted column widths for readability.

Hid less relevant columns for a cleaner layout.

Observations & Recommendations

The First Name column may be redundant if full names are kept.

Adding a Customer Email field would improve order tracking.

Missing city/state values need attention since deliveries are limited to Richland and Hastings.

Tools & Skills

Microsoft Excel

Data cleaning & formatting techniques

Functions: TRIM(), YEAR(), TODAY()

Text to Columns, Find & Replace, Remove Duplicates

Quality control and formatting for usability

File Organization

freedom-rock-cleanup/
├── raw_data/
│   └── employees_raw.xlsx
├── cleaned_data/
│   ├── employees_cleaned.xlsx
│   └── orders_cleaned.xlsx
├── final_reports/
│   ├── salary_bonus_analysis.xlsx
│   └── formatted_orders.xlsx
└── README.md
