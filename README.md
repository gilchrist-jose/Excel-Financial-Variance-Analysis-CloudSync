# Financial Variance Analysis Dashboard | CloudSync Solutions

**Analyst:** Gilchrist Jose  
**Technology Stack:** Microsoft Excel | Power Query
**Domain:** Financial Planning & Analysis (FP&A)  
**Date:** February 2026

---

## 📊 Executive Summary

Interactive financial variance dashboard analyzing $111M in annual financial performance for CloudSync Solutions, a B2B SaaS company. Integrated multiple data sources, resolved data quality issues, and delivered executive ready insights identifying $5.3M revenue outperformance and targeted cost optimization opportunities.

**Dashboard Preview:**

<img width="1825" height="663" alt="image" src="https://github.com/user-attachments/assets/16bba8b8-8a56-412b-a7bd-f92374c78bf0" />

---

## 🎯 Business Context

CloudSync Solutions required systematic monitoring of monthly financial performance against budget to support strategic resource allocation decisions. The analysis needed to accommodate mid year budget revisions, identify one time anomalies, and provide multi dimensional visibility into department and category level variances.

**Key Stakeholders:** CFO, Finance Leadership, Department Heads

---

## 🔧 Technical Architecture

### Data Infrastructure

**Source Systems:**
- Monthly actuals feed (372 transactions across 31 GL accounts)
- Annual budget with Q3 revision cycle (31 accounts × 12 months)

**ETL Pipeline (Power Query):**
```
Source Data (CSV) → Data Quality Validation → Transformation → 
Merge on Composite Key → Calculated Metrics → Load to Data Model
```

**Data Quality Controls Implemented:**
- Null value detection and remediation
- Department/category classification validation
- Account name standardization

**Composite Key Design:**
- Month + Category + Account + Department (ensures accurate budget matching)

---

## 📈 Analytical Framework

### Variance Methodology

**Calculated Metrics:**
- Dollar Variance: `Actual - Budget`
- Percentage Variance: `(Actual - Budget) / Budget`
- Variance Classification (helper column): Context-dependent logic
  - Revenue: Positive variance = Favorable
  - Expenses: Negative variance = Favorable
  -  *Used for data validation and potential filtering*

**Analysis Dimensions:**
- Temporal: Monthly, YTD
- Organizational: Department, Category
- Granularity: Summary → Category → Account detail

**Pivot Table Architecture:**
1. P&L Summary (Category level performance)
2. Time Series (Monthly trend analysis)
3. Department Attribution (Accountability view)
4. Category Deep-Dive (Expense driver identification)
5. Account Detail (Top 15 variance contributors)

---

## 💡 Key Findings

### Financial Performance Overview

**Revenue: Significant Outperformance**
- Actual: $37.9M | Budget: $32.6M | Variance: +$5.3M
- All subscription tiers exceeded targets
- Enterprise segment is strongest performer

**Operating Expenses: Mixed Performance**
- Actual: $73.1M | Budget: $70.1M | Variance: +$1.8M
- Strategic investments in growth initiatives

**Net Position:**
- Net Loss: -$35.3M 
- Revenue trajectory supports scaling strategy

---

### Department Performance

**Top Performers (Under Budget):**
- Engineering: -$65.1K
- Executive: -$0.5K
- Product: -$0.1K

**Attention Required (Over Budget):**
- Operations: +$109.4K
- Customer Success: +$71.8K

---

### Temporal Patterns

- **Jan-Mar:** Seasonal revenue softness
- **Apr-Jun:** Marketing campaign investment spike 
- **Jul-Sep:** Budget revision execution; spending normalization
- **Oct_dec:** Revenue acceleration

---

## 🎨 Dashboard Features

### KPI Summary
- Total Revenue, Expenses, Net Profit/Loss, Revenue Variance, Expense Variance

### Interactive Visualizations
1. **Monthly Trend** (Line Chart): Actual vs Budget trajectory with seasonality
2. **Category Performance** (Column Chart): Variance by P&L category
3. **Department Attribution** (Bar Chart): Accountability by organization
4. **Top Variance Drivers** (Bar Chart): Account-level detail (Top 15)

### Dynamic Filtering
- Department slicer (8 departments)
- Category slicer (5 P&L categories)
- Month slicer (12 months)
- All visualizations respond to filter selections

---

## 🛠️ Technical Capabilities Demonstrated

### Data Engineering
- Multi source ETL with Power Query
- Composite key merge operations
- Data validation and quality controls
- Conditional logic for classification
- Custom calculated columns

### Financial Analysis
- Variance analysis methodology
- Budget vs actual reconciliation
- One time item identification
- Favorable/unfavorable classification with business context
- Mid year budget revision handling

### Business Intelligence
- Executive dashboard design
- Multi dimensional analysis
- Interactive filtering architecture
- KPI selection and visualization
- Insight generation and recommendation development

### Domain Expertise
- SaaS financial model understanding
- P&L structure and account hierarchy
- Budget cycle management
- FP&A reporting standards
- Growth stage investment strategy

---

## 💻 Tools & Technologies

- **Microsoft Excel 2016+**: Data structuring, pivot tables, visualization
- **Power Query**: ETL, data transformation, merge operations
- **Pivot Tables**: Multi dimensional analysis
- **Interactive Dashboards**: Slicer architecture, report connections

---

## 📂 Repository Contents

```
├── README.md
├── CloudSync_Financial_Variance_Analysis_2025.xlsx
├── CloudSync_Actuals_2025.csv
├── CloudSync_Budget_2025.csv
└── CloudSync_Dashboard_Screenshot.png
```

---

## 🚀 Usage Instructions

1. Download Excel workbook
2. Enable Power Query connections if prompted
3. Navigate to Dashboard tab for executive view
4. Use slicers to filter by Department, Category, or Month
5. Review Analysis tab for detailed pivot tables
6. Examine Cleaned_Data tab for merged dataset
7. Access Power Query editor (Data → Queries & Connections) to review transformation logic

---

## 📧 Professional Background

**Gilchrist Jose**  
Data Analyst | Business Intelligence

📁 [GitHub Portfolio](https://github.com/gilchrist-jose)  
💼 [LinkedIn](https://www.linkedin.com/in/gilchrist-jose-a96658322/)  
✉️ gill.christ11@gmail.com

**Related Projects:**
- [Sales Performance Analytics]([https://github.com/gilchrist-jose/TechGear-Sales-Analysis-2025](https://github.com/gilchrist-jose/Excel-Sales-Analysis-TechGear)) - Interactive sales dashboard with trend analysis and KPI tracking

---

## Tags

`Financial-Analysis` `Variance-Analysis` `Power-Query` `Excel` `Budget-Management` `FP&A` `Business-Intelligence` `SaaS-Metrics` `CFO-Reporting` `Data-Modeling` `ETL` `Interactive-Dashboard`
