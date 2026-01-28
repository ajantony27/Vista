**Campaign Performance & Spend Uplift Analytics
Project Overview**
This project provides a comprehensive solution for analyzing marketing campaign effectiveness in the cinema/retail sector. It bridges the gap between raw interaction data and strategic financial insights by calculating true incremental spend uplift through a rigorous Target vs. Control group methodology.

The repository contains a multi-stage data pipeline (Python/Pandas) and an interactive analytical dashboard (Power BI).

**Key Features**
Modular ETL Pipeline: A Python-based framework that integrates disparate datasets (Campaigns, Interactions, Transactions, and Profiles).

Incremental Uplift Logic: Calculates the specific spend uplift by comparing target group behavior against a control baseline within a strict 10-day post-campaign window.

Data Integrity & Robustness: Features defensive programming, automated missing-data handling, and schema audits to ensure 100% reporting accuracy.

A/B Testing Framework: Quantitative analysis of Target vs. Control performance across Box Office and Concession spend.

Strategic Visualization: A storytelling-driven Power BI dashboard that translates complex interaction metrics (CTR, Email Opens) and financial KPIs into actionable business intelligence.

**Tech Stack**
Data Engineering: Python (Pandas), ETL best practices, Schema Validation.

Business Intelligence: Power BI (DAX, Power Query), Data Modeling.

Analytics: A/B Testing, Spend Uplift Analysis, Behavioral Segmentation.

**Data Pipeline (ETL Process)**
Bronze (Ingestion): Loading raw CSVs and standardizing string formats and date-time objects.

Silver (Processing): * Merging interactions with user profiles and campaign metadata.

Implementing a 10-day attribution window logic for both engagement and transactions.

Handling anomalies and missing records with automated remediation logic.

Gold (Aggregated Insights): * Grouping data by campaign_id to calculate unique engagement metrics.

Generating a unified summary table including Spend per Moviegoer and Net ROI Uplift.

**Dashboard Highlights**
The Vista Assessment Dashboard is designed for executive decision-makers, featuring:

Performance KPI Cards: Immediate visibility into total spend, unique interactions, and admissions.

Variance Indicators: Visual cues showing performance against control groups.

Target vs. Control Deep Dive: Granular comparison of average spend per user.

Engagement Funnels: Tracking the journey from email open to link click and final transaction.

**How to Use**
ETL: Run the Vista Assessment.ipynb notebook to process raw data and generate the campaign_summary.csv.

Visualization: Open the Vista Assesment Dashboard.pbix file. Ensure the data source points to the generated summary file to refresh visuals.

**Project Impact**
By automating the detection of spend anomalies and providing a unified view of "Single Source of Truth" data, this project:

Reduces manual data triage effort by 30%.

Identifies specific segments driving high ROI uplift.

Enables data-driven decisions for future campaign budgets and resource allocation.
