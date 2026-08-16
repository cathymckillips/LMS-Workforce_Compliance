# LMS-Workforce_Compliance
This project demonstrates how HR and Learning Management System data can be transformed into actionable reporting.

**Power BI | SQL Server | SQL | DAX | Python | Data Quality | MDM**

An end-to-end healthcare workforce and Learning Management System (LMS) analytics project designed to demonstrate reporting, training compliance monitoring, data-quality validation, Master Data Management (MDM), and operational analytics.

> **Data Disclaimer:** All data used in this project is synthetic and was created solely for portfolio and demonstration purposes. No real employee, patient, healthcare organization, LMS, or confidential business data is included.

---

## 📌 Project Overview

I developed this **LMS & Workforce Compliance Analytics** project to demonstrate how HR and Learning Management System data can be transformed into actionable reporting for training compliance, workforce operations, data quality, and Master Data Management.

The project simulates a healthcare training and workforce reporting environment and focuses on real-world reporting activities such as:

- Monitoring required training compliance
- Identifying overdue and upcoming training
- Investigating cross-system data discrepancies
- Detecting missing and duplicate records
- Reviewing duplicate Party IDs
- Supporting MDM merge workflows
- Maintaining recurring weekly reporting
- Providing operational work queues for analysts

Rather than building Power BI visuals directly from raw files, the project uses a multi-layer reporting architecture:

**Python → SQL Server → SQL Reporting Views → Data Validation → Historical Snapshots → Power BI**

---

## 🎯 Business Problem

HR, workforce, and training teams need reliable information to answer questions such as:

- What is the current required-training compliance rate?
- Which employees, departments, locations, or courses require attention?
- How much training is overdue?
- What training is approaching its due date?
- Are LMS records consistent with workforce data?
- Which records contain missing, duplicate, or invalid information?
- Which MDM Party IDs require duplicate or merge review?
- How is training compliance changing over time?

The goal of this project was to create a reporting solution that supports both **leadership-level monitoring** and **analyst-level investigation**.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **Python** | Generated synthetic HR, LMS, course, and MDM datasets |
| **SQL Server / SSMS** | Data storage, transformation, validation, and reporting |
| **SQL** | Joins, aggregations, data-quality rules, views, and troubleshooting |
| **SQL Views** | Created reporting-ready datasets for Power BI |
| **SQL History Table** | Preserved recurring compliance snapshots |
| **Power BI** | Data modeling, DAX, visualization, filtering, and reporting |
| **DAX** | Dynamic KPIs, compliance calculations, and exception metrics |

---

## 🏗️ Solution Architecture

```text
Synthetic Data Generation
        │
        ▼
      Python
        │
        ▼
    CSV Files
        │
        ▼
   SQL Server
        │
        ├── HR Workforce Data
        ├── LMS Training Assignments
        ├── Course Catalog
        └── MDM Party ID Data
        │
        ▼
 SQL Reporting Layer
        │
        ├── Employee Training
        ├── Training Compliance
        ├── Data Quality Exceptions
        ├── MDM Duplicate Review
        └── Weekly Compliance
        │
        ▼
Historical Compliance Snapshots
        │
        ▼
     Power BI
        │
        ├── Compliance Overview
        ├── Training Detail
        ├── Data Quality
        ├── MDM Review
        └── Report Documentation
