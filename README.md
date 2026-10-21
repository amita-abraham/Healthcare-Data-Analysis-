# Healthcare Data Analysis and Insights 📊🏥

## 📌 Project Overview

The healthcare industry generates large volumes of data related to patient health, medical history, hospital services, and healthcare expenses. Analyzing this data can help identify patterns, understand patient health profiles, and support data-driven decision-making.

**Healthcare Data Analysis and Insights** is an Excel-based data analytics project that explores relationships between patient demographics, medical conditions, hospitalization details, and healthcare charges. The project focuses on data cleaning, transformation, exploratory data analysis, pivot tables, data visualization, and interactive dashboard development using Microsoft Excel.

## 🎯 Project Objectives

- Clean and prepare healthcare data by identifying and handling missing values.
- Transform raw data into structured, analysis-ready information.
- Categorize patients based on BMI and HbA1C levels.
- Combine multiple datasets using Customer ID.
- Analyze relationships between health indicators, medical history, and healthcare charges.
- Create visualizations to identify trends and patterns.
- Develop an interactive dashboard with slicers for dynamic data exploration.

## 🛠️ Tools and Technologies

- **Microsoft Excel**
- VLOOKUP for data integration
- Excel formulas for data cleaning and transformation
- Pivot Tables and Pivot Charts
- Pie and Donut Charts
- Column and Bar Charts
- Line and Scatter Plots
- Interactive Dashboard and Slicers

## 📂 Dataset Description

The project uses a healthcare dataset consisting of three tables:

1. **Medical Examinations** – Contains patient health indicators such as BMI, HbA1C, heart issues, transplant history, cancer history, smoking status, and number of major surgeries.
2. **Hospitalization Details** – Includes hospitalization-related information such as date components, healthcare charges, hospital tier, city tier, and state ID.
3. **Customer Names** – Contains customer identification and name information.

The tables were integrated using **Customer ID** as the common key to create a consolidated healthcare dataset for analysis.

## 🔄 Project Workflow

### 1. Data Cleaning

- Identified missing values represented by `?` in the Medical Examinations and Hospitalization Details tables.
- Replaced missing month values with `Sep`.
- Imputed missing year values using the rounded average year.
- Filled missing smoker, Hospital tier, and City tier values using the respective most frequent values.
- Handled missing State ID values by substituting it with "Unknown"

### 2. Data Transformation

- Split customer names into Title, First Name, and Last Name.
- Converted the NumberOfMajorSurgeries column into numerical values by standardizing non-numeric entries.
- Checked Heart Issues and smoker columns for inconsistent values.
- Created a **Weight Status** column using BMI categories:
  - Underweight
  - Normal Weight
  - Overweight
  - Obesity
- Created a **Diabetes Status** column using HbA1C categories:
  - Normal
  - Prediabetes
  - Diabetes
- Combined year, month, and date into a formatted Date of Birth column.
- Calculated customer age as of June 8, 2023.
- Formatted healthcare charges as currency.

### 3. Data Integration

Created a consolidated worksheet named **Healthcare** by combining the three tables using VLOOKUP and Customer ID.

The final dataset retained the following fields:

- Customer ID
- First Name
- BMI
- HbA1C
- Heart Issues
- Any Transplants
- Cancer History
- NumberOfMajorSurgeries
- Smoker
- Weight Status
- Diabetes Status
- Date of Birth
- Charges
- Hospital Tier
- City Tier
- State ID
- Age

### 4. Data Analysis and Visualization

Used Pivot Tables and charts to investigate the following questions:

**A. Medical History and Lifestyle**
- Examined the distribution of cancer history among smokers and non-smokers.
- Compared the total number of major surgeries and average HbA1C levels between patients with and without a history of transplants.

**B. Healthcare Charges**
- Analyzed healthcare charges across different weight statuses and diabetes statuses.
- Compared average healthcare charges across hospital tiers within different states.

**C. Age and Health Indicators**
- Explored the relationship between age and BMI.
- Examined the relationship between age and HbA1C.
- Investigated the relationship between age and healthcare charges.

### 5. Interactive Dashboard

Developed an Excel dashboard to consolidate the key visualizations and make the analysis easier to interpret.

**Dashboard features:**
- Multiple chart types for comparing health indicators and healthcare costs.
- Pivot Chart-based visualizations for exploring patterns in the dataset.
- Interactive slicers for Weight Status and Diabetes Status.
- Dynamic filtering to compare healthcare outcomes and charges across patient categories.

## 📈 Key Analysis Areas

The project enables exploration of:

- Smoking status and cancer history.
- Transplant history, major surgeries, and HbA1C levels.
- BMI and diabetes categories in relation to healthcare charges.
- Differences in average charges across hospital tiers and states.
- Associations between age, BMI, HbA1C, and healthcare expenses.

The dashboard supports interactive exploration of these relationships, helping users identify patterns that may warrant further investigation.

## 💡 Skills Demonstrated

- Data Cleaning and Missing Value Handling
- Data Transformation and Feature Creation
- Data Integration using VLOOKUP
- Excel Formulas and Conditional Logic
- Exploratory Data Analysis (EDA)
- Pivot Tables and Pivot Charts
- Healthcare Data Analysis
- Data Visualization
- Interactive Dashboard Development
- Analytical Thinking and Data Interpretation

## 📁 Project Structure

```text
Healthcare-Data-Analysis-and-Insights/
│
├── Healthcare Data Analysis - ME Assignment.xlsx
└── README.md
```

## 🚀 How to Use

1. Clone or download this repository.
2. Open the Excel workbook in Microsoft Excel.
3. Navigate to the consolidated Healthcare worksheet to explore the prepared dataset.
4. Open the dashboard worksheet to view the visualizations.
5. Use the Weight Status and Diabetes Status slicers to filter and explore the data interactively.

## ⚠️ Limitations

- Findings depend on the completeness and quality of the available dataset.
- Missing-value imputation and data standardization decisions may influence the results.
- Observed relationships and correlations do not establish causation.
- BMI and HbA1C categories are analytical classifications and should not be treated as independent clinical diagnoses.
- Healthcare charges may be influenced by factors not included in the dataset.

## 👩‍💻 Conclusion

This project demonstrates how Microsoft Excel can be used to transform raw healthcare data into structured information and interactive visual insights. Through data cleaning, transformation, integration, analysis, and dashboard creation, the project provides a practical foundation for understanding patient health profiles and exploring healthcare cost patterns.

It also demonstrates the application of core data analytics skills to a healthcare use case, supporting the development of data-driven insights for further investigation and decision-making.
