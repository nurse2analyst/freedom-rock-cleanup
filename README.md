# Freedom Rock Bicycles: Data Cleanup (Excel Project)

## Overview  
This project demonstrates Excel-based data cleaning and organization for employee and order records at Freedom Rock Bicycles. The goal was to turn messy, inconsistent data into a clean, reliable dataset ready for reporting and decision-making.  

---

## Files  
- **Raw Data**  [freedomrock_raw_2025.xlsx](https://github.com/user-attachments/files/22412086/freedomrock_raw_2025.xlsx)

- **Cleaned Data**  [freedomrock_clean_2025.xlsx](https://github.com/user-attachments/files/22412089/freedomrock_clean_2025.xlsx)


---

## Key Work  

### Employees Data  
- Removed duplicates and corrected errors  
- Standardized state, city, phone numbers, and job titles  
- Added calculated fields for years of service and salary with bonus  

### Orders Data  
- Split comma-separated values into columns  
- Reformatted order dates and headers  
- Split full names into first/last name  
- Improved layout for readability  

---

## Insights & Recommendations  
- Some order records are missing location details (critical for delivery).  
- A customer email field would improve

## Skills Used  
- Microsoft Excel  
- Data cleaning and standardization  
- Functions: `TRIM()`, `YEAR()`, `TODAY()`  
- Text to Columns, Remove Duplicates, Find & Replace  

---

## 📁 Project Structure  
freedom-rock-cleanup/
├── raw_data/ # Original files
├── cleaned_data/ # Cleaned employee & order data
├── final_reports/ # Salary analysis & formatted orders
└── README.md
