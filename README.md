# 👥 HR Analytics Dashboard (Power BI)

> An end-to-end Power BI project focused on analyzing Human Resources (HR) data to uncover insights into employee demographics, attrition, job satisfaction, compensation, and workforce trends.

---

# 📖 Project Overview

This project aims to build an interactive HR Analytics dashboard using Microsoft Power BI.

The project follows a structured Business Intelligence workflow, beginning with importing the dataset, cleaning and transforming the data using Power Query, building a relational data model, creating DAX measures, and finally designing an interactive dashboard.

Each major milestone is maintained in a separate Git branch to demonstrate an organized and version-controlled development process.

---

# 📈 Current Progress

## ✅ Completed

- Created the Power BI project.
- Imported the HR Analytics dataset.
- Performed data quality assessment.
- Removed missing values.
- Removed duplicate records.
- Corrected spelling inconsistencies.
- Validated data types.
- Loaded the cleaned dataset into Power BI.
- Designed the dashboard header.
- Applied a consistent report theme and colour palette.
- Added dashboard branding with a custom logo.
- Created the Total Employees KPI card.
- Created the Active Employees KPI card.
- Created a calculated **AttritionCount** column using Power Query.
- Developed the Attrition Count KPI card.
- Created the Attrition Rate (%) DAX measure.
- Developed the Attrition Rate (%) KPI card.
- Created the Average Age KPI card.
- Created the Average Experience KPI card.
- Developed the first analytical visualization showing employee attrition by department.
- Developed the Attrition by Salary Slab clustered bar chart.
- Developed the Attrition by Job Role & Job Satisfaction matrix visualization.

## 🔄 Next Steps

- Build charts and visualizations.
- Finalize dashboard layout.

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

# 🎨 Dashboard Design

After preparing and cleaning the dataset, the next stage of the project focused on designing the user interface for the HR Analytics dashboard.

The objective was to create a clean, modern, and professional dashboard layout that provides a strong visual foundation for presenting HR insights.

---

## 🖥 Dashboard Header

The first component designed was the dashboard header.

The following customizations were applied:

### 📐 Header Container

- Added a **Text Box** to serve as the dashboard header.
- Set the dimensions to:
  - **Width:** 1259 px
  - **Height:** 85 px

---

### 🎨 Background Styling

Applied a professional corporate theme using:

| Property | Value |
|----------|-------|
| Background Color | `#1F3A8A` |
| Transparency | `0%` |

---

### 📝 Header Title

Configured the dashboard title with the following formatting:

| Property | Value |
|----------|-------|
| Text | **HR ANALYTICS DASHBOARD** |
| Font Size | 36 |
| Font Color | White |
| Font Weight | Bold |
| Text Alignment | Center |

---

### ⬜ Border Styling

Enhanced the header appearance by enabling a visual border.

| Property | Value |
|----------|-------|
| Border | Enabled |
| Corner Radius | 12 px |
| Border Color | `#E6E6E6` |

---

### 🌑 Shadow Effect

Added a subtle shadow to create depth and improve visual hierarchy.

| Property | Value |
|----------|-------|
| Shadow | Enabled |
| Shadow Color | `#B3B3B3` |

---

### 🖼 Dashboard Branding

Added a company-style logo to the left side of the dashboard title to improve branding and overall visual appeal.

---

### 🎨 Dashboard Canvas

Configured the report page background with a soft neutral color.

| Property | Value |
|----------|-------|
| Background Color | `#EEF1F7` |
| Transparency | `0%` |

The selected color palette provides strong contrast while maintaining a clean and professional Business Intelligence dashboard aesthetic.

---

# 📊 KPI Card Development

Following the completion of the dashboard layout and branding, the next phase focused on designing the dashboard's **Key Performance Indicator (KPI)** cards.

KPIs provide users with a quick overview of important workforce metrics and serve as the primary summary indicators displayed at the top of the dashboard.

The first two KPI cards developed were:

- 👥 Total Employees
- ✅ Active Employees

---

## 👥 KPI 1 — Total Employees

A **Card** visual was added from the **Visualizations** pane to display the total number of employees within the organization.

The **EmpID** field was assigned to the card and its aggregation was configured to **Count**, allowing Power BI to calculate the total number of employee records.

### Card Dimensions

| Property | Value |
|----------|-------|
| Width | **197 px** |
| Height | **104 px** |

---

### Card Position

| Property | Value |
|----------|-------|
| Horizontal | **10 px** |
| Vertical | **95 px** |

---

### Card Title

The card title was configured to improve readability and maintain consistency across the dashboard.

| Property | Value |
|----------|-------|
| Title | **Total Employees** |
| Font Size | **20** |
| Font Weight | **Bold** |
| Alignment | **Center** |

---

### Card Styling

The following visual styling was applied to create a clean and modern KPI card.

| Property | Value |
|----------|-------|
| Background Color | `#F5F8FF` |
| Border | Enabled |
| Border Color | `#D9DEE7` |
| Corner Radius | **12 px** |
| Shadow | Enabled |

These settings create a card-like appearance while maintaining consistency with the overall dashboard theme.

---

### Callout Value

The card value was formatted to improve visibility.

| Property | Value |
|----------|-------|
| Label | Hidden |
| Font Size | **25** |
| Font Weight | **Bold** |
| Alignment | **Right** |

Additionally, the **Inner Border** was disabled to produce a cleaner visual presentation.

---

## ✅ KPI 2 — Active Employees

The second KPI card was created by duplicating the **Total Employees** card to ensure consistent formatting and alignment.

The duplicated card was modified to display the total number of **active employees**.

### Configuration

- Changed the title to **Active Employees**.
- Used the employee count measure based on **EmpID**.
- Applied a visual filter where:

| Field | Condition |
|--------|-----------|
| Attrition | **No** |

This filter excludes employees who have left the organization, allowing the card to display only the current active workforce.

---

## 📉 KPI 3 – Attrition Count

To calculate the total number of employees who have left the organisation, a new calculated column was first created in **Power Query**.

### Creating the AttritionCount Column

The **EmpID** field was selected and **Transform Data** was used to open the **Power Query Editor**.

From the **Add Column** tab, a **Conditional Column** was created with the following configuration:

| Property | Value |
|----------|-------|
| Column Name | **AttritionCount** |
| Condition | If **Attrition = "Yes"** then **1**, otherwise **0** |

The resulting Power Query expression was:

```powerquery
= Table.AddColumn(
    #"Changed Type1",
    "AttritionCount",
    each if [Attrition] = "Yes" then 1 else 0
)
```

This transformation creates a binary indicator that assigns:

- **1** → Employee has left the organisation.
- **0** → Employee is currently employed.

After applying the transformation:

- The changes were loaded into Power BI using **Close & Apply**.
- The **AttritionCount** column data type was updated to **Whole Number** using the **Column Tools** tab.

---

### Creating the KPI Card

A new **Card** visual was added to display the total number of employees who have left the organisation.

Configuration:

- Title: **Attrition Count**
- Value: **Sum of AttritionCount**
- Verified that **Filters on this visual** remained set to **(All)** to ensure all employee records were included in the calculation.

This KPI provides an overall count of employee attrition across the organisation.

---

## 📊 KPI 4 – Attrition Rate (%)

To better understand employee turnover, a DAX measure was created to calculate the overall attrition rate.

### DAX Measure

The following measure was created:

```DAX
Attrition Rate % =
DIVIDE(
    SUM('hr-data'[AttritionCount]),
    SUM('hr-data'[EmployeeCount]),
    0
)
```

The measure was then formatted as:

| Property | Value |
|----------|-------|
| Format | Percentage |
| Decimal Places | **1** |

A new KPI card was created with:

- Title: **Attrition Rate %**
- Value: **Attrition Rate %** (DAX Measure)

Using the **DIVIDE()** function ensures that division-by-zero errors are handled safely while returning an accurate percentage.

---

## 👤 KPI 5 – Average Age

A KPI card was created to display the average employee age.

Configuration:

| Property | Value |
|----------|-------|
| Title | **Average Age** |
| Field | **Age** |
| Aggregation | **Average** |

This KPI provides a quick overview of the average workforce age.

---

## 💼 KPI 6 – Average Experience

The final KPI card was developed to display the average employee tenure within the organisation.

Configuration:

| Property | Value |
|----------|-------|
| Title | **Avg Experience** |
| Field | **YearsAtCompany** |
| Aggregation | **Average** |

This KPI highlights the average number of years employees have remained with the organisation.

---

## 🎨 KPI Enhancements

To improve dashboard readability and visual appeal, custom icons will be added to each KPI card in the next stage of development.

These icons will provide users with immediate visual recognition of each business metric while maintaining a consistent dashboard theme.

---

## 📈 Dashboard Progress

At this stage, the dashboard includes the following KPI cards:

- 👥 Total Employees
- ✅ Active Employees
- ❌ Attrition Count
- 📉 Attrition Rate (%)
- 👤 Average Age
- 💼 Average Experience

Together, these KPIs provide a high-level summary of the organisation's workforce and establish the foundation for the analytical dashboard.

The next phase of development will focus on designing interactive charts, visualisations, and additional analytical components.

---

---

# 📈 Data Visualization Development

With the dashboard KPIs completed, the next phase of the project focused on developing interactive visualizations to provide deeper insights into workforce attrition.

The first visualization created was a **Donut Chart**, allowing users to quickly compare employee attrition across different departments.

---

## 🍩 Visualization 1 – Attrition by Department

A **Donut Chart** visual was added from the **Visualizations** pane to display the distribution of employee attrition across each department.

### Data Configuration

The following fields were assigned to the chart.

| Field | Assignment |
|--------|------------|
| Legend | **Department** |
| Values | **Sum of AttritionCount** |

Using the **AttritionCount** column ensures that only employees who have left the organisation are included in the visualization.

---

### Visual Dimensions

To maintain a balanced dashboard layout, the visual was positioned beneath the KPI cards using the following dimensions.

| Property | Value |
|----------|-------|
| Width | **350 px** |
| Height | **249 px** |
| Horizontal Position | **179 px** |
| Vertical Position | **210 px** |

---

### Chart Title

The chart title was updated to clearly describe the information being presented.

| Property | Value |
|----------|-------|
| Title | **Attrition by Department** |
| Font Weight | **Bold** |

---

### Visual Styling

To maintain consistency across the dashboard, the chart was formatted using the same design language as the KPI cards.

| Property | Value |
|----------|-------|
| Visual Border | Enabled |
| Border Colour | `#D9DEE7` |
| Corner Radius | **12 px** |
| Shadow | Enabled |

Applying identical styling creates a consistent and professional user interface throughout the report.

---

### Legend Formatting

The legend was customised to improve readability.

The following formatting was applied:

- Legend Title: **Disabled**
- Font Weight: **Bold**
- Text Colour: **Black**

Removing the legend title reduces unnecessary visual clutter while keeping the department names clear and easy to read.

---

### Detail Labels

The detail labels were formatted to provide concise information without overcrowding the chart.

| Property | Value |
|----------|-------|
| Font Size | **10** |
| Font Weight | **Bold** |
| Text Colour | **Black** |
| Value Decimal Places | **0** |
| Percentage Decimal Places | **0** |

Displaying both employee counts and percentages enables users to compare departments quickly while maintaining readability.

---



---

## 📊 Visualization 2 – Attrition by Salary Slab

The second visualization was developed to analyze employee attrition across different salary ranges within the organisation.

A **Clustered Bar Chart** was selected as it provides an effective comparison of employee counts across salary slabs while also allowing attrition status to be displayed using colour coding.

---

### Data Configuration

The following fields were assigned to the visual.

| Field | Assignment |
|--------|------------|
| Y-Axis | **SalarySlab** |
| X-Axis | **Count of EmpID** |
| Legend | **Attrition** |

Using **Count of EmpID** allows the chart to display the number of employees within each salary range, while the legend separates employees based on their attrition status.

---

### Visual Dimensions

The visual was positioned alongside the department visualization to maintain a balanced dashboard layout.

| Property | Value |
|----------|-------|
| Width | **355 px** |
| Height | **251 px** |
| Horizontal Position | **537 px** |
| Vertical Position | **209 px** |

---

### Chart Title

The title was updated to clearly communicate the purpose of the visualization.

| Property | Value |
|----------|-------|
| Title | **Attrition by Salary Slab** |

---

### Consistent Dashboard Styling

To maintain a consistent dashboard appearance, the **Format Painter** tool was used.

Rather than manually reapplying formatting, the styling from the **Attrition by Department** donut chart was copied and applied to the clustered bar chart.

This ensured consistency across:

- Border styling
- Rounded corners
- Shadow effects
- Background formatting
- Overall visual design

Using the **Format Painter** also improves development efficiency while maintaining a uniform dashboard theme.

---

### Axis & Legend Formatting

Several formatting improvements were applied to improve readability.

#### Y-Axis

- Font Weight: **Bold**
- Text Colour: **Black**

#### Legend

- Position: **Bottom Centre**

Using the **Attrition** field as the legend allows users to compare employees who remained with the organisation against those who left across each salary slab.

---

### Data Labels

Data labels were enabled to improve readability and reduce the need to reference axis values.

The following formatting was applied:

| Property | Value |
|----------|-------|
| Data Labels | Enabled |
| X-Axis Values | Hidden |

Displaying values directly on each bar allows users to interpret the visualization more quickly while reducing unnecessary visual clutter.

---

---

## 📋 Visualization 3 – Attrition by Job Role & Job Satisfaction

The third visualization was developed to analyse employee attrition across different job roles while simultaneously comparing employee job satisfaction levels.

A **Matrix** visual was selected because it provides a compact way of displaying multiple dimensions within a single report, allowing users to compare attrition counts across both job roles and satisfaction ratings.

---

### Data Configuration

The following fields were assigned to the matrix.

| Field | Assignment |
|--------|------------|
| Rows | **JobRole** |
| Columns | **JobSatisfaction** |
| Values | **Sum of AttritionCount** |

Using the **AttritionCount** field ensures that the matrix displays only employees who have left the organisation, while the **JobSatisfaction** column enables comparisons across satisfaction levels for each job role.

---

### Visual Dimensions

To maintain a balanced dashboard layout, the matrix was positioned alongside the existing visualizations.

| Property | Value |
|----------|-------|
| Width | **371 px** |
| Height | **251 px** |
| Horizontal Position | **898 px** |
| Vertical Position | **209 px** |

---

### Chart Title

The title was updated to clearly describe the purpose of the visualization.

| Property | Value |
|----------|-------|
| Title | **Attrition by Job Role & Job Satisfaction** |

---

### Consistent Dashboard Styling

To maintain a consistent visual theme throughout the dashboard, the **Format Painter** tool was used.

Formatting from the previously created visualization was copied and applied to the matrix visual, ensuring consistency across:

- Border styling
- Rounded corners
- Shadow effects
- Background formatting
- Overall dashboard appearance

Applying identical formatting improves dashboard consistency while reducing repetitive formatting work.

---

### Conditional Formatting

To improve data interpretation, **Background Colour** was enabled within **Cell Elements**.

Conditional formatting automatically highlights values using colour intensity, making it easier to identify job roles with comparatively higher or lower employee attrition across different job satisfaction levels.

---

### Header Formatting

Both column and row headers were customised to improve readability.

#### Column Headers

| Property | Value |
|----------|-------|
| Font Weight | **Bold** |
| Text Colour | **Black** |

#### Row Headers

| Property | Value |
|----------|-------|
| Font Weight | **Bold** |
| Text Colour | **Black** |
| Text Size | **9** |

Reducing the row header text size allows more job roles to be displayed while maintaining a clean and compact layout.

---

## 📊 Business Insight

This visualization provides a multi-dimensional view of employee attrition by combining job role with job satisfaction levels.

It enables users to identify whether particular job roles experience higher attrition within specific satisfaction ratings, helping HR teams uncover potential relationships between employee satisfaction and workforce turnover.

---

## 📊 Business Insight

This visualization helps identify how employee attrition varies across different salary ranges.

By combining salary information with attrition status, users can quickly determine whether employee turnover is concentrated within specific salary bands, supporting workforce planning and compensation analysis.

---

## 📊 Business Insight

This visualization highlights how employee attrition is distributed across departments, making it easier to identify which departments contribute the largest proportion of employee turnover.

Combined with the KPI cards developed previously, this chart provides additional context by moving from overall workforce metrics to department-level analysis.

---

## 📈 Dashboard Progress

## 📈 Dashboard Progress

The dashboard currently includes:

- Dashboard branding and report theme.
- Six workforce KPI cards.
- Attrition by Department donut chart.
- Attrition by Salary Slab clustered bar chart.
- Attrition by Job Role & Job Satisfaction matrix.
- Consistent dashboard styling and formatting.

The next stage of development will focus on creating additional analytical visualizations, report slicers, filters, and interactive dashboard components.

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

# 📈 Current Status

The HR Analytics dashboard now includes a professionally designed dashboard interface, six workforce KPI cards, and three analytical visualizations.

Current accomplishments include:

- Data preparation and transformation using Power Query.
- Dashboard branding and report theme customization.
- KPI development using Power BI Cards.
- Creation of analytical visualizations for departmental attrition, salary-based attrition, and job role satisfaction analysis.

The next stage of development will focus on creating additional analytical visualizations, report slicers, interactive filtering, and dashboard refinement.

---

# 🚀 Future Development

The remaining stages of the project include:

- Additional interactive charts and visualizations
- Dashboard slicers and filters
- Advanced DAX measures
- Workforce demographics analysis
- Employee performance insights
- Dashboard optimization and refinement

---

# 📬 Contact

If you have any questions, suggestions, or feedback regarding this project, feel free to open an issue or connect with me on GitHub.

---

# ⭐ Support

If you found this project useful or interesting, consider giving the repository a **⭐ Star**.
