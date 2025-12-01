# 📊 Market Data Analysis in Power BI

### A Data-Driven Exploration of Job Roles, Skills, Salaries & Companies

## 📘 Overview

### This project analyzes job market data using Power BI, focusing on job positions, salaries, skills, experience levels, and company characteristics.
Originally based on a DataCamp dataset, the project expands on it with extensive data cleaning, modeling, DAX calculations, and dashboard design.

###The final report includes four interactive dashboards—Jobs, Skills, Company, and Home—each equipped with slicers and cross-filtering for deeper exploration.

## 🛠️ Tools Used

Power BI Desktop
Power Query
DAX (Data Analysis Expressions)
Data Modeling
Interactive Dashboards

📂 Dataset Fields
🧑‍💼 Job Information
Job Title
Job Title Additional Info
Job Position Type
Job Position Level
Years of Experience
Job Skills
Min Pay / Max Pay
Pay Rate

📅 Job Posting Details

Job Posting ID

Job Posting Date

Number of Applicants

🏢 Company Information

Company Name

Company Industry

Company Size

Job Location

🧹 Data Preparation (Power Query)
Column Profiling

Switched profiling from Top 1000 rows to Entire Dataset

Reviewed:

Missing values

Distinct & unique values

Column distribution

Summary statistics

Skill Cleaning

Created a new table using only Job Posting ID and Job Skills

Removed:

Brackets

Quotes

Extra spaces

Split skills by delimiter into new rows

Removed empty rows

Standardized naming (ex: powerbi → power_bi)
