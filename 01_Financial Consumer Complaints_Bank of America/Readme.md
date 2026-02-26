# Bank of America — Financial Consumer Complaints Analysis
### CFPB Public Data | 2017–2023 | 62,516 Records

---

## Project Overview

This project analyzes 62,516 consumer complaints filed against Bank of America 
with the Consumer Financial Protection Bureau (CFPB) between 2017 and 2023. 
Findings are benchmarked against the CFPB Consumer Response Annual Report 2023 
to evaluate Bank of America's performance relative to industry standards.

---

## Business Questions Answered

1. Do consumer complaints show any seasonal patterns?
2. Which products present the most complaints and what are their most common issues?
3. How are complaints typically resolved?
4. What can we learn from complaints with untimely responses?

---

## Dataset

| Attribute | Value |
|---|---|
| Source | Maven Analytics (CFPB Public Domain) |
| Company | Bank of America |
| Time Period | Year 2017 to 2023 |
| Records | 62,516 |
| Fields | 12 original + 7 helper columns added |
| Reference | CFPB Consumer Response Annual Report 2023 |

---

## Key Findings

### 1. Seasonal Patterns
- July 2023 = 1,749 complaints — highest single month in the dataset
- Checking/savings account surge (51% of July volume) drove the spike
- Consistent with CFPB 2023 findings on peer-to-peer unauthorized transactions
- 2020 did NOT show the industry-wide COVID forbearance dip

### 2. Product & Issue Breakdown
- Checking/savings = 39.7% of all complaints vs 79% credit reporting industry-wide
- "Managing an account" = 15,109 complaints — 24% of the entire dataset
- Two products (checking/savings + credit card) = 65.6% of all complaints

### 3. Resolution Quality
- Overall monetary relief = 23.5% vs 1.5% industry average — misleading headline
- At product level: credit card 7.7% vs 15% industry — 50% below benchmark
- No product where Bank of America exceeds industry monetary relief benchmark

### 4. Untimely Response Risk
- Overall untimely rate = 3.94% — 4x the industry average
- Debt collection (6.44%) and credit reporting (6.32%) = highest regulatory risk
- Mortgage (0.24%) = standout performer below industry average

---

## Methodology

### Tools Used
- Data Analysis: Microsoft Excel — data cleaning, pivot tables, charts, dashboard
- Presentation: Canva

### Data Cleaning Steps
- Duplicated raw sheet — preserved original as audit trail
- Created 7 helper columns: Year, Month Number, Month Name, 
  Days-to-Route, Resolution Category, Relief Given, 
- Audited blank fields using `COUNTBLANK` across critical columns
- Validated date formats and converted where necessary

### Analysis Framework
- 4 pivot tables answering 4 business questions
- `COUNTIFS` for filtered segment analysis
- Benchmarked all findings against CFPB 2023 Annual Report

---

## Dashboard Preview

![Dashboard](visuals/dashboard_overview.png)

---

## Repository Structure
```
├── README.md
├── data/
│   └── file name
├── analysis/
│   └── file name
├── excel/
│   └── file name
├── visuals/
│   ├── file name.png
│   ├── file name.png
│   ├── file name.png
│   └── file name.png
├── presentation/
│   └── file name.pdf
└── references/
    └── cfpb_report_notes.md
```

---

## References

- [CFPB Consumer Response Annual Report 2023]
  (https://www.consumerfinance.gov)
- [Maven Analytics Dataset — Financial Consumer Complaints]
  (https://mavenanalytics.io)
- [Storytelling with Data (2015) by Cole Nussbaumer Knaflic](https://amzn.to/3DZNzOv)

---

## Author

Rishabh Bahuguna
[LinkedIn](https://www.linkedin.com/in/rishabhbahuguna03)  
[GitHub](https://www.github.com/Rishabhbahuguna03)