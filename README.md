# HealthConnect Clinic — Appointment No-Show Analysis

**AnalystLab Africa Experience Lab | Data Analytics Track — Week 4 (Project Kickoff)**

## 📌 Project Overview

HealthConnect Clinic is a fictional healthcare provider facing a significant operational challenge: a high rate of missed appointments (no-shows), which leads to inefficient use of appointment slots, repetitive administrative burden, and reduced quality of patient care.

**Central Project Question:** *How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?*

This is a shared, multi-track Experience Lab project. Each intern track (Data Analytics, Data Science, Machine Learning Engineering, Generative AI, Project Management) contributes from its own professional angle. This repository documents the **Data Analytics track** contribution, progressing week by week toward a portfolio-ready final deliverable.

> ⚠️ Week 4 is a foundation stage. The focus is on problem understanding, resource review, and initial planning — not on final analysis, dashboards, or models.

## 🗂️ Repository Structure

```
├
├── Initial_Analysis_Document.docx     # Dataset overview, data quality assessment, business questions, potential KPIs
├── Week4_Project_Summary.docx         # Concise summary of Week 4 progress and Week 5 focus
└── README.md
```
*(Structure will expand in subsequent weeks as the project progresses through Analysis & Solution Design, Development, Testing, and Final Presentation.)*

## 📊 Dataset

**File:** `HealthConnect_Appointment_Data.csv` (5,000 fictional, anonymized appointment records, 18 variables)

Covers: patient demographics, appointment details, booking information, previous appointment/no-show history, reminder information, distance to clinic, waiting time, and appointment outcome (target variable: `Attended` / `No-Show` / `Cancelled`).

## 🔍 Week 4 — Key Findings

| Metric | Value |
|---|---|
| Total appointments | 5,000 |
| Total variables | 18 |
| Duplicate records | 0 |
| **Overall no-show rate** | **48.46%** (2,423 of 5,000) |
| Attended | 46.28% (2,314) |
| Cancelled | 5.26% (263) |
| Missing values — `reminder_channel` | 27.32% (likely structural: no reminder sent → no channel) |
| Missing values — `distance_to_clinic_km` | 1.80% |
| Missing values — `waiting_time_minutes` | 1.20% |

**Headline insight:** Nearly one in two appointments results in a no-show — a rate well above typical healthcare industry benchmarks (10–30%), confirming the business problem is significant and worth investigating in depth.

## ❓ Business Questions (Week 4)

1. What is the overall no-show rate, and how does it vary by patient/appointment characteristics?
2. Does sending a reminder (and its channel) reduce the no-show rate?
3. Does booking lead time affect the likelihood of a no-show?
4. Do patients with a history of no-shows repeat the pattern?
5. Does distance to the clinic influence attendance?
6. Are certain appointment types, days, or time slots more prone to no-shows?

## 📈 Potential KPIs Identified (not yet calculated — Week 5 scope)

1. Overall No-Show Rate
2. No-Show Rate by Reminder Status (sent vs. not sent)
3. No-Show Rate by Booking Lead Time band
4. No-Show Rate by Patient No-Show History (`previous_no_shows`)
5. No-Show Rate by Distance to Clinic band

Each KPI is explicitly linked to one of the business questions above; full justification is documented in `Initial_Analysis_Document.docx`.

## 🛠️ Tools & Techniques (planned)

- Python (pandas, matplotlib) or Power BI for exploratory and business analysis
- Data cleaning: recoding of `reminder_channel`, handling of marginal missing values, date consistency checks

## ▶️ Next Steps (Week 5)

- Calculate the 5 identified KPIs and build supporting visualizations.
- Identify the 2–3 factors most strongly associated with no-shows.
- Formulate initial, evidence-based recommendations for clinic management.

## 👤 Author

Josfrid AGBADOGBE, Data Analytics Intern, AnalystLab Africa Experience Lab
*Week 4 — HealthConnect Project Kickoff & Problem Understanding*
