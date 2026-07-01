# 🏦 Bank Loan Analysis using Microsoft Fabric & Power BI

### 📖 Project Overview

This project is an end-to-end **Bank Loan Analysis** solution built using **Microsoft Fabric, Lakehouse, PySpark, and Power BI**. It analyzes customer loan data to identify approval trends, customer demographics, income patterns, and financial behavior. The project follows the **Bronze → Silver → Gold** architecture to transform raw data into business-ready insights.

---

### 🎯 Business Objective

- Analyze customer loan applications.
- Identify factors influencing loan approvals.
- Monitor customer income and mortgage trends.
- Compare approved and rejected loans.
- Build an interactive dashboard for business decision-making.

---

### 🛠️ Technologies Used

- Microsoft Fabric
- OneLake
- Lakehouse
- PySpark
- Power BI
- Power Query
- DAX
- Microsoft Excel

---

### 📂 Project Architecture

```
Excel Dataset
      │
      ▼
Microsoft Fabric
      │
      ▼
OneLake
      │
      ▼
Lakehouse
      │
      ▼
Bronze Layer
(Raw Data)
      │
      ▼
Silver Layer
(Cleaned Data)
      │
      ▼
Gold Layer
(Business Data)
      │
      ▼
Semantic Model
      │
      ▼
Power BI Dashboard
```

---

### 🔄 ETL Process

#### 🥉 Bronze Layer
- Imported raw Excel data into the Lakehouse.
- Stored the source data without any transformations.

#### 🥈 Silver Layer
- Cleaned and validated the data.
- Corrected data types.
- Removed duplicate records.
- Handled missing values.
- Standardized column names.

#### 🥇 Gold Layer
- Prepared analytics-ready data.
- Created business-friendly columns.
- Optimized data for reporting.
- Loaded the final dataset into the Semantic Model.

---

### 📊 Dashboard Features

#### KPI Cards
- Total Customers
- Loan Approved
- Loan Rejected
- Loan Approval Rate
- Average Income
- Average Mortgage
- Average Credit Card Spending
- Online Banking Customers
- Credit Card Customers

#### Visualizations
- Loan Approval by Age Group
- Loan Approval by Education
- Income Analysis
- Loan Status Distribution
- Family Size Analysis
- Mortgage Analysis
- Online Banking Analysis
- Credit Card Analysis

---

### 📈 DAX Measures

- Total Customers
- Loan Approved
- Loan Rejected
- Loan Approval Rate
- Average Income
- Average Mortgage
- Total Income
- Average Credit Card Spending
- Online Banking Customers
- Credit Card Customers

---

### 💡 Business Insights

- Customers with higher income have a greater chance of loan approval.
- Professional and graduate customers show higher loan acceptance.
- Customers with CD Accounts are more likely to take personal loans.
- Online banking users represent a large customer segment.
- Mortgage values influence loan approval decisions.

---

### ⚠️ Challenges Faced

**Challenge**

During the Bronze-to-Silver transformation, the **Date** column displayed **NULL** values after conversion.

**Root Cause**

The source Excel file stored dates as **string (text)** values, and PySpark could not directly convert them into the Date data type.

**Solution**

- Verified the schema using `printSchema()`.
- Identified the correct date format.
- Converted the string values into the Date data type.
- Validated the transformed data before loading it into the Silver layer.

**Result**

The Date column was successfully converted, and all records were loaded correctly into the Silver layer.

---

### 📁 Repository Structure

```
Bank-Loan-Analysis
│
├── Dataset
│   └── Bank_Personal_Loan_Modelling.xlsx
│
├── Notebooks
│   ├── Bronze_to_Silver.ipynb
│   └── Silver_to_Gold.ipynb
│
├── Power BI Report
│   └── Bank Loan Analysis.pbix
│
├── Dashboard Screenshots
│
└── README.md
```

---

### 🚀 Project Outcome

- Built an end-to-end Microsoft Fabric data pipeline.
- Implemented the Bronze, Silver, and Gold architecture.
- Created an interactive Power BI dashboard with business KPIs.
- Delivered actionable insights to support loan approval decisions.
- Demonstrated practical Data Engineering and Business Intelligence skills.

---

### 📸 Dashboard Preview

<img width="672" height="388" alt="Screenshot 2026-06-27 142851" src="https://github.com/user-attachments/assets/60d5f392-b690-414e-9848-7a1c756596a6" />


---

### 👩‍💻 Author

**Mythili Maram**

**Aspiring Data Engineer**

**Skills:** Microsoft Fabric | Power BI | PySpark | SQL | Python | Azure
