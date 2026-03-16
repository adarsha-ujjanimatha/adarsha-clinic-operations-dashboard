# Adarsha Clinic — Ayurvedic Clinic Operations Dashboard

## Overview
End-to-end data analytics project for a solo Ayurvedic clinic in Harapanahalli, Karnataka, India. Designed a relational database, wrote 20 SQL queries (basic to advanced), and built visualisations using Python and Tableau analysing 24 months of clinic operations.

## Business Problem
The clinic maintained all patient records on paper with zero digital tracking. No visibility into patient trends, revenue patterns, Panchakarma therapy completion rates, or seasonal disease patterns.

## Dataset
| Table | Rows | Description |
|-------|------|-------------|
| patients | 3,000 | Patient demographics, Prakriti (Ayurvedic constitution) |
| visits | 8,977 | Consultations with Ayurvedic diagnosis and prescriptions |
| billing | 8,977 | Revenue, payment methods, discounts |
| panchakarma_sessions | 8,789 | Individual therapy session tracking with completion status |
| therapy_pricing | 9 | Therapy rates and package pricing |

**Period:** January 2024 – December 2025 (24 months)  
**Total Rows:** 30,000+

## Tools & Skills
- **MySQL** — Relational database design, JOINs, CTEs, Window Functions (LAG, RANK, Running Totals), CASE WHEN
- **Python** — Pandas, Matplotlib, Seaborn for data analysis and visualisation
- **Jupyter Notebook** — Full documented analysis with 20 queries and charts
- **Tableau Public** — Interactive 4-page dashboard with cross-filtering
- **Data Analysis** — Seasonal trend analysis, patient retention, revenue forecasting

## Key Findings
1. **Joint Pain & Back Pain = top diagnoses** with seasonal spikes during winter/monsoon (Vata dosha aggravation)
2. **Panchakarma completion rate ~65%** — incomplete packages represent significant lost revenue
3. **UPI digital payments grew from ~15% to ~60%** over 24 months
4. **Year-over-year revenue growth of ~15%** — healthy business trajectory
5. **Monday = busiest day** — opportunity to optimise scheduling and staffing

## SQL Queries (20 Total)
| Level | Queries | Techniques |
|-------|---------|------------|
| Basic (1-5) | Patient counts, gender split, diagnosis frequency, revenue trends, payment methods | GROUP BY, COUNT, SUM, AVG |
| Intermediate (6-10) | Revenue split, patient lifetime value, therapy popularity, visit type analysis | JOINs, CASE WHEN, CONCAT |
| Advanced (11-20) | MoM growth, retention rates, seasonal patterns, lost revenue, UPI trends | CTEs, Window Functions, Running Totals, DATEDIFF |

## Dashboard
[View Interactive Dashboard on Tableau Public](PASTE_YOUR_TABLEAU_LINK_HERE)

### Page 1: Patient Overview
![Patient Overview](screenshots/dashboard_page1.png)

### Page 2: Revenue Analytics
![Revenue Analytics](screenshots/dashboard_page2.png)

### Page 3: Clinical & Panchakarma Insights
![Clinical Insights](screenshots/dashboard_page3.png)

### Page 4: Clinic Performance
![Clinic Performance](screenshots/dashboard_page4.png)

## Recommendations
1. Implement WhatsApp/SMS reminders for Panchakarma follow-up sessions
2. Offer 5-10% completion discount to incentivise full therapy course adherence
3. Expand morning Panchakarma slots (higher revenue per visit)
4. Stock top 10 most prescribed Ayurvedic medicines at the clinic
5. Adopt a digital patient management system to replace paper records

## Project Structure
```
├── data/                    # Dataset (5 CSV files, 30,000+ rows)
│   ├── patients.csv
│   ├── visits.csv
│   ├── billing.csv
│   ├── panchakarma_sessions.csv
│   └── therapy_pricing.csv
├── sql/
│   ├── 01_create_tables.sql
│   ├── 02_basic_queries.sql
│   ├── 03_intermediate_queries.sql
│   └── 04_advanced_queries.sql
├── screenshots/             # Tableau dashboard screenshots
├── Adarsha_Clinic_Operations_Analysis.ipynb  # Jupyter Notebook
├── Adarsha_Clinic_Operations_Analysis.pdf    # PDF Report
└── README.md
```

## Author
**Adarsha Ujjanimatha**  
MSc Data Science & Analytics — Cardiff University (2024)  
