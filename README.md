# freedom-rock-cleanup
Excel project demonstrating data cleaning, column transformations, and calculated fields for employee and order records.
[freedomrock_raw_2025.xlsx](https://github.com/user-attachments/files/21559352/freedomrock_raw_2025.xlsx)
[freedomrock_clean_2025.xlsx](https://github.com/user-attachments/files/21559354/freedomrock_clean_2025.xlsx)
# Freedom Rock Bicycles: Employee & Order Data Cleanup (Excel Project)

## 📌 Project Overview
As a new data analyst at Freedom Rock Bicycles, I was tasked with cleaning and organizing employee and order data that had been inconsistently managed by previous staff. The goal was to improve data accuracy, formatting, and usability for reporting and decision-making.

This project involved two worksheets:
- **Employees**: Staff records requiring cleaning, standardization, and calculated fields.
- **Orders**: Delivery order data that needed parsing, formatting, and review for quality control.

---

## 🧾 Tasks Completed

### 🧑‍💼 Employees Worksheet
- ✅ Removed duplicate records using **Remove Duplicates**
- ✅ Center-aligned the values in the **Bonus %** column
- ✅ Capitalized all state abbreviations in the **State** column
- ✅ Trimmed extra spaces from the **City** column using the `=TRIM()` function
- ✅ Replaced the outdated job title "Salesman" with "Salesperson" using **Find and Replace**
- ✅ Performed **spell check** to correct any misspellings (excluding street names and employee names)
- ✅ Moved the **City** column to appear before **State**
- ✅ Corrected missing data in multiple fields
- ✅ Standardized phone numbers to use a consistent area code format: `(###) ###-####`
- ✅ Added a new column **"Years"** to calculate tenure using the formula:  
  `=YEAR(TODAY()) - YEAR(Hire Date)`
- ✅ Added and calculated a new column **"Salary with Bonus"** using:  
  `=Salary * (1 + Bonus %)`

---

### 🚲 Orders Worksheet
- ✅ Parsed a comma-separated file using **Text to Columns**
- ✅ Formatted the **Order Date** column (Column B) as **Short Date**
- ✅ Bolded and center-aligned all column headers
- ✅ Split employee full names into **First Name** and **Last Name** columns using `Text to Columns`
- ✅ Adjusted all column widths for better visibility
- ✅ Hid the **First Name** column for cleaner presentation

---

## 🧠 Analytical Insights

### 🔍 Unnecessary Column
- The **"First Name"** column may not be necessary in future orders if the full name is still retained elsewhere.

### ➕ Recommended Column
- The manager should consider adding a **"Customer Email"** field to improve order tracking and communication.

### ❌ Missing Data
- Several entries were missing required location information, such as city or state — critical since deliveries are limited to **Richland** and **Hastings** only.

---

## 🛠️ Tools & Skills Used
- Microsoft Excel
- Data cleaning techniques
- Text to Columns
- Formulas: `TRIM()`, `YEAR()`, `TODAY()`, calculated fields
- Formatting (alignment, font styles, column width)
- Find & Replace
- Spell check and quality control

---

## 📁 File Structure
freedom-rock-cleanup/
├── raw_data/
│ └── employees_raw.xlsx
├── cleaned_data/
│ └── employees_cleaned.xlsx
│ └── orders_cleaned.xlsx
├── final_reports/
│ └── salary_bonus_analysis.xlsx
│ └── formatted_orders.xlsx
└── README.md
