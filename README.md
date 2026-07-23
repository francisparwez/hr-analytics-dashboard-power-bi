# 👥 HR Analytics Dashboard (Power BI)

> An end-to-end Power BI project focused on analyzing Human Resources (HR) data to uncover insights into employee demographics, attrition, job satisfaction, compensation, and workforce trends.

---

# 📖 Project Overview

This project aims to build an interactive HR Analytics dashboard using Microsoft Power BI.

The project follows a structured Business Intelligence workflow, beginning with importing the dataset, cleaning and transforming the data using Power Query, building a relational data model, creating DAX measures, and finally designing an interactive dashboard.

Each major milestone is maintained in a separate Git branch to demonstrate an organized and version-controlled development process.

---

# 🚧 Current Progress

## ✅ Completed

- Created the Power BI project.
- Imported the HR Analytics dataset.
- Performed data quality assessment.
- Cleaned and transformed the dataset using Power Query.
- Loaded the cleaned dataset into Power BI.

## 🔄 Upcoming

- Build the relational data model.
- Create DAX measures.
- Design the interactive dashboard.
- Generate business insights.

---

# 📂 Repository Structure

```text
HR-Analytics-Dashboard/
│
├── data/
│   └── hr-data.csv
│
├── hr-analytics-dashboard.pbix
│
└── README.md
```

---

# 📊 Dataset Information

The project uses a Human Resources dataset containing employee-related information for workforce analytics.

## Dataset Summary

| Property | Value |
|----------|-------|
| File Name | `hr-data.csv` |
| Original Rows | 1,480 |
| Columns | 37 |
| Format | CSV |

---

# 📋 Dataset Features

The dataset contains employee information including:

- Employee ID
- Age
- Age Group
- Attrition
- Business Travel
- Department
- Distance From Home
- Education
- Education Field
- Environment Satisfaction
- Gender
- Job Involvement
- Job Level
- Job Role
- Job Satisfaction
- Marital Status
- Monthly Income
- Salary Slab
- Hourly Rate
- Overtime
- Performance Rating
- Relationship Satisfaction
- Stock Option Level
- Total Working Years
- Work-Life Balance
- Years at Company
- Years in Current Role
- Years Since Last Promotion
- Years With Current Manager

These fields will later be used to build KPIs and business intelligence reports.

---

# 🧹 Data Cleaning & Transformation

The dataset was cleaned and prepared using **Power Query Editor** before loading it into the Power BI data model.

The following data quality checks and transformations were performed:

### ✔️ Column Quality Assessment

- Used **Column Quality** to identify empty values and data errors across all columns.
- Verified that the dataset contained no data errors.

---

### ✔️ Handling Missing Values

The **YearsWithCurrManager** column contained approximately **6% null values**.

To address this:

- Sorted the column in ascending order to bring null values to the top.
- Counted the affected rows.
- Identified the first **61 rows** as containing null values.
- Removed these rows from the dataset.

---

### ✔️ Duplicate Removal

- Checked the dataset for duplicate records.
- Identified **16 duplicate rows**.
- Removed all duplicate records to improve data integrity.

---

### ✔️ Correcting Spelling Inconsistencies

The **BusinessTravel** column contained inconsistent category values:

| Before | After |
|---------|-------|
| Travel_Rarely | TravelRarely |

All instances of **Travel_Rarely** were standardized to **TravelRarely** to ensure consistent reporting and filtering.

---

### ✔️ Data Type Validation

Reviewed each column to verify that the assigned data type matched the data it contained.

Examples include:

- Whole Number
- Decimal Number
- Text
- True/False

This ensures accurate calculations and visualizations throughout the project.

---

### ✔️ Load Cleaned Dataset

After completing all cleaning and validation steps, the dataset was loaded into Power BI using the **Close & Apply** option.

---

# 🎯 Project Objectives

The completed dashboard will help answer questions such as:

- What is the employee attrition rate?
- Which departments experience the highest turnover?
- Which job roles have the greatest attrition?
- How does salary influence employee retention?
- What is the distribution of employees across departments?
- How do job satisfaction and work-life balance vary?
- What are the workforce demographics?

---

# 🌿 Git Branch Workflow

| Branch | Description |
|----------|-------------|
| `01-blank-project` | Initial Power BI project setup |
| `02-importing-dataset_transforming-it` | Imported, cleaned, and transformed the HR dataset using Power Query *(Current Branch)* |
| `03-building-relational-model` | Create the relational data model |
| `04-add-dax-measures` | Create KPIs and business metrics |
| `05-designing-dynamic-dashboard` | Design the final interactive dashboard |
| `main` | Final completed project |

---

# 🛠 Technologies Used

- Microsoft Power BI
- Power Query
- Git
- GitHub

---

# 📈 Current Status

The HR dataset has been successfully:

- Imported into Power BI.
- Cleaned using Power Query.
- Validated for missing values, duplicates, spelling inconsistencies, and data types.
- Loaded into the Power BI model for the next stage of development.

The next phase of the project will focus on building the relational data model.

---

# 🚀 Future Development

The completed project will include:

- Relational Data Model
- DAX Measures
- KPI Cards
- Interactive Filters
- Employee Attrition Analysis
- Workforce Demographics
- Department Performance Analysis
- HR Analytics Dashboard

---

# 📬 Contact

If you have any questions, suggestions, or feedback regarding this project, feel free to open an issue or connect with me on GitHub.

---

# ⭐ Support

If you found this project useful or interesting, consider giving the repository a **⭐ Star**.