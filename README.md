# Azure Data Factory – SCD Type 2 Implementation

## 📌 Project Overview

This project demonstrates an end-to-end implementation of Slowly Changing Dimension (SCD Type 2) using:

- Azure Data Factory (Mapping Data Flows)
- Azure SQL Database
- Conditional Split
- Join Transformation
- Derived Columns
- Alter Row Policies
- Surrogate Key Management

---

## 🏗 Architecture Flow

1. Source – Customer Raw Data  
2. Data Cleaning (Derived Column)  
3. Conditional Split (Valid / Invalid Records)  
4. Error Handling Sink  
5. Left Outer Join with Dimension Table  
6. Change Detection Logic  
7. Alter Row Policies (Insert / Update)  
8. Final Sink – Dim_Customer  

---

## 🔁 SCD Type 2 Logic

- New records → Insert
- Changed records → Expire old record + Insert new version
- Unchanged records → No action
- Surrogate key generated automatically
- EffectiveStartDate & EffectiveEndDate maintained
- IsCurrent flag maintained

---

## 💡 Skills Demonstrated

- Azure Data Factory
- Mapping Data Flows
- Data Transformation
- SCD Type 2 Implementation
- Data Warehousing Concepts
- Surrogate Key Strategy
- Error Handling in ETL
- Azure SQL Integration

---

## 🚀 Author

Abdul Kareem  
Aspiring Cloud Data Engineer  
GitHub: https://github.com/abkareem831013
