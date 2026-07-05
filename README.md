# SAP Procure-to-Pay (P2P) Risk Analytics Dashboard

## Overview

This repository contains my internship project completed at **Ernst & Young (EY)** in the Risk Advisory practice. The project focuses on designing an end-to-end **SAP Procure-to-Pay (P2P) Risk Analytics solution** that identifies procurement, payment, and vendor master data risks using **Power BI**, **Excel**, and **SAP business logic**.

The objective of this project was to replicate a real-world consulting engagement by transforming business requirements into interactive dashboards capable of monitoring procurement exceptions and highlighting financial exposure.

---

<img width="516" height="398" alt="Screenshot 2026-07-05 183709" src="https://github.com/user-attachments/assets/64ec644e-8cf0-4ccf-87c0-59c9b0566aee" />
<img width="518" height="398" alt="Screenshot 2026-07-05 183048" src="https://github.com/user-attachments/assets/12a23be2-7fad-463e-985c-e001a2253516" />

(Additional dashboard screenshots for all six scenarios are available in the Screenshots/ folder.)


## Project Workflow

The project followed the complete analytics lifecycle typically adopted in consulting engagements:

1. Understanding the Procure-to-Pay (P2P) business process
2. Preparing Business Requirement Documents (BRDs)
3. Designing synthetic SAP datasets
4. Validating business logic using Excel Pivot Tables
5. Building interactive Power BI dashboards
6. Performing business analysis and identifying control gaps
7. Documenting insights and recommendations

---

## Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel
- SAP Business Logic

---

## SAP Tables Used

The project was designed using the structure of standard SAP ERP tables, including:

- EKKO – Purchasing Document Header
- EKPO – Purchasing Document Item
- EKBE – Purchase Order History
- LFA1 – Vendor Master (General)
- LFB1 – Vendor Master (Company Code)
- BSIK – Vendor Open Items
- BSAK – Vendor Cleared Items

---

# Risk Scenarios Covered

## 1. Purchase Price Variance

Identifies inconsistent pricing for the same material under different procurement conditions.

Sub-scenarios:
- Same Material, Same Plant, Same Vendor
- Same Material, Same Plant, Different Vendor
- Same Material, Different Plant, Same Vendor
- Same Material, Different Plant, Different Vendor

Key Analysis:
- Financial impact
- Price variance %
- Exception grouping
- Procurement trends
- Vendor drill-down

---

## 2. Purchase Order Tolerance Analysis

Evaluates inconsistencies in over-delivery and under-delivery tolerances defined in purchase orders.

Sub-scenarios:
- Multiple tolerance values for the same material and vendor
- Invalid tolerance defined for discrete units of measure

Key Analysis:
- Exception distribution
- Material-wise exceptions
- Tolerance profiles
- Financial impact

---

## 3. Multiple Payment Terms

Detects vendors assigned multiple payment terms across purchase orders.

Key Analysis:
- Vendor-wise payment term mapping
- Financial exposure
- Exception distribution
- Vendor-level drillthrough

---

## 4. Vendor Master Validation

Performs master data quality checks.

Checks include:
- Invalid PAN format
- Invalid GST format
- Duplicate PAN
- Duplicate GST

Key Analysis:
- Duplicate vendor identification
- PAN/GST validation
- Vendor master health indicators

---

## 5. Duplicate Payment Detection

Identifies potential duplicate invoice postings.

Sub-scenarios:
- Same Vendor
- Different Vendor

Key Analysis:
- Duplicate exposure
- Vendor-wise impact
- Invoice-level drillthrough
- Financial trend

---

## 6. Three-Way Match Compliance

Compares:

- Purchase Order Quantity
- Goods Receipt Quantity
- Invoice Quantity

Classification:
- Match
- PO-GRN Mismatch
- GRN-Invoice Mismatch
- All Three Mismatch

Key Analysis:
- Compliance %
- Financial impact
- Vendor-wise exposure
- Quantity comparison

---

# Dashboard Features

The Power BI solution includes:

- Interactive KPI Cards
- Dynamic Slicers
- Drillthrough Pages
- Custom Tooltip Pages
- Cross-filtering
- Decomposition Analysis
- Financial Impact Analysis
- Exception Investigation Tables
- Trend Analysis
- Vendor-wise Risk Monitoring

---

# Validation Methodology

Before dashboard development, **all business exceptions were first identified and validated using Microsoft Excel Pivot Tables**. Each scenario was independently verified against the Business Requirement Document (BRD) to ensure that the implemented business logic, exception counts, and financial impact calculations were accurate before building the Power BI dashboards.

---

# Business Requirement Documentation (BRD)

Each scenario was first documented through a formal Business Requirement Document containing:

- Objective
- Business Risk
- Business Impact
- SAP Tables
- SAP Fields
- Business Logic
- Exception Criteria

This documentation served as the blueprint for dataset creation and dashboard development.

---

# Repository Structure

## Repository Structure

```text
P2P-Risk-Analytics-Dashboard
│
├── README.md
│
├── Documentation
│   ├── Internship P2P Project Report.pdf
│   └── BRD P2P Process.xlsx
│
├── Dashboards
│   └── Scenario Dashboard.pbix
│
├── Datasets
│   ├── P2P Scenario 1 - Price Variance Dataset.xlsx
│   ├── P2P Scenario 2 - PO Tolerance Dataset.xlsx
│   ├── P2P Scenario 3 - Multiple Payment Terms Dataset.xlsx
│   ├── P2P Scenario 4 - Vendor Master Check Dataset.xlsx
│   ├── P2P Scenario 5 - Duplicate Payment Risk Dataset.xlsx
│   └── P2P Scenario 6 - 3 Way Match Compliance Dataset.xlsx
│
├── Pivot Table Analysis
│   ├── P2P Scenario 1 (Price Variance) Pivot Table Analysis.xlsx
│   ├── P2P Scenario 2 (PO Tolerance) Pivot Table Analysis.xlsx
│   ├── P2P Scenario 3 (Multiple Payment Terms) Pivot Table Analysis.xlsx
│   ├── P2P Scenario 4 (Vendor Master Check) Pivot Table Analysis.xlsx
│   ├── P2P Scenario 5 (Duplicate Payment Risk) Pivot Table Analysis.xlsx
│   └── P2P Scenario 6 (3 Way Match Compliance) Pivot Table Analysis.xlsx
│
├── Screenshots
│   ├── Price Variance Dashboard.png
│   ├── PO Tolerance Dashboard.png
│   ├── Multiple Payment Terms Dashboard.png
│   ├── Vendor Master Check Dashboard.png
│   ├── Duplicate Payment Risks Dashboard.png
│   ├── 3 Way Match Compliance Dashboard.png
│   ├── Tooltip Example.png
│   └── Drillthrough Example.png
│
└── Presentation
    └── Procurement to Pay Process.pptx
```
# Key Learning Outcomes

Through this project, I gained practical experience in:

- SAP Procure-to-Pay process understanding
- Procurement risk analytics
- Business Requirement Documentation
- SAP table relationships
- Excel-based data validation
- Power Query transformations
- DAX calculations
- Interactive dashboard development
- Business reporting
- Financial risk analysis
- Data storytelling
- Control monitoring

---

# Disclaimer

This project uses **synthetically generated datasets** created solely for learning and demonstration purposes.

No confidential client information or proprietary EY data has been used.

The SAP table structures and business scenarios are based on industry-standard Procure-to-Pay practices.

---

## Author

**Khushi Jain**

SAP Procure-to-Pay Risk Analytics Internship Project

Ernst & Young (EY)

Power BI | SAP | Excel | Risk Analytics
