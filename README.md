# 📊 Market Data Analysis in Power BI

### A Data-Driven Exploration of Job Roles, Skills, Salaries & Companies

## 📘 Overview

This project analyzes job market data using Power BI, focusing on job positions, salaries, skills, experience levels, and company characteristics.

Originally based on a DataCamp dataset, the project expands on it with extensive data cleaning, modeling, DAX calculations, and dashboard design.

The final report includes four interactive dashboards—Jobs, Skills, Company, and Home—each equipped with slicers and cross-filtering for deeper exploration.

## 🛠️ Tools Used

Power BI Desktop

Power Query

DAX (Data Analysis Expressions)

Data Modeling

Interactive Dashboards

## 📂 Dataset Fields

### 🧑‍💼 Job Information

Job Title Full: The full title for the job position

Job Title: The simplified title for the job position 

Job Title Additional Info: Any additional information for a job title

Job Position Type: The time/job requirements

Job Position Level: Indicates seniority of a job position

Years of Experience: The number of years of experience

Job Skills: List of skill requirements

Min Pay / Max Pay: The highest & Lowest salary/pay offered

Pay Rate: The rate of pay for the job

### 📅 Job Posting Details

Job Posting ID: The unique identification number for each job posting

Job Posting Date: The date of the job posting

Number of Applicants: The number of those that applied for the job in the first 24 hours

### 🏢 Company Information

Company Name: The name of the company sponsoring the job

Company Industry: The industry that the company is involved

Company Size: The size of the company by the number of employees

Job Location: The geographic location of the company and job

## 🧹 Data Preparation (Power Query)

### Column Profiling
Switched profiling from Top 1000 rows to Entire Dataset

Reviewed:

Missing values

Distinct & unique values

Column distribution

Summary statistics

### Skill Cleaning

Created a new table using only Job Posting ID and Job Skills

Removed:

Brackets

Quotes

Extra spaces

Split skills by delimiter into new rows

Removed empty rows

Standardized naming (ex: powerbi → power_bi)

## 🧮 DAX Calculations

### Measures Table

Average of Average Pay = AVERAGE('Job Postings'[Average Pay])

Posting Count = COUNT('Job Postings'[Job Posting ID])

Posting Count = COUNT('Job Postings'[Job Posting ID])

% Skill in Posting = [Skill Count] / [Posting Count]

## 📑 Report Pages

### Job Level Analysis

Bar chart: Average Years of Experience by Job Position Level

Stacked area chart: Count of JOb POsting ID by Year, Quarter, Month and Job Position Level

### Job Titles

Treemap: Count of Job Skills by Job Title and Job Skills

### Salary Analysis

Line Chart: Average of Average Pay by Years of Experience and Job Title

### Skill Analysis

Stacked Column Chart: Count of Job Skills by Job Skills

### Skill Likelihood

Line Chart: % Skill in Posting by Year, Quarter, and Job Skills

Table: Job Skills, Job Title, % Skill in Posting

Filters: Job Title, Job Skills

### Experience Analysis

Scatter Plot: Average of Years of Experience, Posting Count and Posting Count by Job Position Level and Company Industry

Stacked Column Chart: Skill Count by Company Industry (Top 10 by Posting Count)

Scatter Plot: Average of Years of Experience and Posting Count by Company Size

Scatter Plot: Average of Years of Experience and Posting Count by Company Industry

Table: Job Title, Company Name, Posting Count

## 🏠 Dashboards

### Home Dashboard

Clickable bookmarks linking to all dashboards

### Jobs Dashboard

Includes visuals from Job Level Analysis & Job Titles

Slicers:

Job Title

Job Position Level

Company Name

Company Size

Company Industry

Job Posting Date

Cards:

Posting Count

Average Years of Experience

### Skills Dashboard

Includes visuals from Skill Analysis

Cards:

Distinct Count of Job Skills

Distinct Count of Job Postings Containing Skill

### Company Dashboard

Includes visuals from Experience Analysis

Gauge Card:

Displays Average Minimum Pay → Average Maximum Pay
