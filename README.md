# Massachusettes-General-Hospital-Analysis

## Description
A data analysis project for Massachusettes General Hospital, conducted as part of the STC 6-Week Data Analyst Mentorship. The project includes data cleaning, analysis, visualization, and actionable recommendations.

## Table of Contents
1. [Introduction](#introduction)  
2. [Project Description](#project-description)  
3. [Project Aim](#project-aim)  
4. [About the Dataset](#about-the-dataset)
5. [Tools Used](#tools-used)  
6. [Importing the Dataset](#importing-the-dataset)  
7. [Data Cleaning and Transformation](#data-cleaning-and-transformation)  
8. [Data Modeling](#data-modeling)  
9. [Data Analysis](#data-analysis)  
10. [Data Visualization](#data-visualization)  
11. [Key Insights](#key-insights)  
12. [Recommendations](#recommendations)  
13. [Conclusion](#conclusion)
14. [Contact Information](#contact-information)

## Introduction
This project analyzes synthetic medical records from Massachusetts General Hospital (2011–2022) to investigate key operational challenges including high patient readmission rates, prolonged hospital stays, elevated procedure costs, and insufficient insurance coverage. The goal is to uncover data-driven insights that support better decision-making, reduce healthcare costs, enhance patient outcomes, and improve the hospital’s overall resource efficiency through effective patient care strategies and optimized hospital operations.

## Project Description
The scope of this project focuses on analyzing synthetic medical records from Massachusetts General Hospital between 2011 and 2022 to understand key operational and clinical challenges. The analysis covers patient demographics, readmission patterns, length of stay, procedure costs, and insurance coverage gaps. It also examines how these factors affect patient outcomes, hospital efficiency, and overall resource utilization, with the goal of identifying high-risk groups, cost drivers, and areas where care delivery can be optimized.

The approach involves a structured workflow beginning with comprehensive data cleaning and preparation to ensure consistency and accuracy across the dataset. Exploratory data analysis (EDA) is then performed to uncover trends, correlations, and anomalies that guide deeper investigation. Using statistical analysis and visualization techniques, the project identifies patterns related to readmissions, costs, and service utilization. Finally, insights are summarized into actionable recommendations to help the hospital reduce operational costs, improve patient outcomes, and allocate resources more efficiently.

## Project Aim
The main objective of this project is to analyze medical records collected internally from the hospital between 2011 and 2022 to provide solutions that guide better decision-making thus answering key business questions such as:
* What are the total and average hospital costs by year and procedure type?
* What are the top 5 most expensive procedures and encounters?
* What is the average length of stay per procedure and encounter?
* What encounter and procedure is causing the longest stay?
* How does the average length of stay vary across encounters and age groups?
* Which year recorded the highest claim and base costs by procedure and encounter?
* Is there a relationship between encounter length of stay (LOS) and total claim cost?
* Which payer has the highest insurance coverage?
* Number of insured patients and uninsured patients
* Number of patients readmitted
* What is the readmission rate?

## About the Dataset
This dataset contains synthetic medical records from Massachusetts General Hospital between 2011 and 2022. It covers approximately 1,000 patients and includes details on hospital visits, procedures, insurance coverage, and patient demographics.

There are 5 main datasets:  
* Patient Table – Contains patient-level details like age, gender, and ID.
* Encounter Table – Records each hospital visit (inpatient, outpatient, emergency, etc.), including admission and discharge dates, costs, and readmission details.
* Payer Table – Contains information about the patient’s insurance coverage or lack of it.
* Procedure Table – Records the medical procedures done during each encounter, linked by IDs.
* Dictionary Table – A reference table to decode procedure categories and types.  

## Tools Used
Microsoft Excel | Power BI

## Importing the Dataset
The datasets were imported as a CSV file into Excel for cleaning. Duplicate copy was created for each before launching Power Query for transformation. After which the datasets were loaded into Power BI for analysis and visualization

## Data Cleaning and Transformation
* Removed duplicates
* Changes column names for clarity e.g. patient to patient id, encounters to encounter id, id to payer id in payers table
* Changes column type (base cost) to currency in procedure table
* Converted all text-based date to actual date format
* Standardized gender values to male and female
* Standardized marital values to single and married
* Standardized entries in the state headquarter column in the payers table

## Data Modeling
* Created a measure called average lenght of stay
* Created a new column with cleaned encounter date
* Extracted the years in the date column into a new column

## Data Analysis
Key Performance Indicators (KPIs) analyzed:
* Total Patients
* Total Readmitted Patients
* Total Encounters
* Total Encounter Claim Cost
* Total Paid Out of Pocket
* Total Insurance Coverage
* Readmission Rate
* Insured Patients
* Uninsured Patients

## Data Visualization
A four-page dashboard was created:
* Masachusettes Hospital Dashboard (page 1)
* Length of Stay Analysis (page 2)
* Cost Analysis (page 3)
* Insurance and Readmission Analysis (page 4)
### Masachusettes Hospital Dashboard
* KPI Cards: Total Patients, Total Readmitted Patients, Total Encounters, Total Encounter Claim Cost, Total Paid Out of Pocket, Total Insurance Coverage
* Bar Chart: Top 5 Encounter Type by Total Claim Cost, Top 5 Procedure Type by Total Base Cost
* Column Chart: Avg Encounter Claim Cost by Age Group, Avg Encounter LOS (days) by Age Group
* Line Chart: Total Encounter Claim Cost by Month
* Slicer: Yearly Trends
### Length of Stay Analysis
* KPI Cards: Avg Encounter LOS (days), Avg Procedure LOS (days)
* Bar Chart: Top 20 Procedure by Avg LOS (days), Top 10 Encounter Type by Avg LOS (days)
* Column Chart: Avg Encounter LOS (days) by Encounter Class, Avg Encounter LOS (days) by Age Group
* Scattered Plot: Relationship btw LOS and Claim Cost by Encounter
### Cost Analysis
*	KPI Cards: Total Procedure Base Cost, Total Encounter Base Cost, Total Encounter Claim Cost, Total Paid Out of Pocket, Avg Paid out of Pocket, Avg Encounter Claim Cost, Avg Encounter Base Cost, Avg Procedure Base Cost
*	Donut Chart: Avg Encounter Claim Cost by Gender
*	Bar Chart: Top 10 Procedure Type by Avg Base Cost, Top 10 Encounter Type by Avg Claim Cost
*	Line Chart: Total Procedre Base Cost by Month
*	Slicer: Yearly Trend
### Insurance and Readmission Analysis
*	KPI Cards: Total Patients, Insured Patients, Uninsured Patients, Total Encounter Claim Cost, Total Insurance Coverage, Total Paid Out of Pocket, Readmission Rate, Total Readmitted Patients
*	Bar Chart: Top 10 Encounter Type by Total Payer Coverage, Top 10 Encounter Type by Total Paid Out of Pocket
*	Column Chart: Top 3 Payers by Total Coverage, Avg Paid Out of Pocket by Age Group
*	Donut Chart: Encounter by Insurannce Coverage
### View Dashboards
<img width="1422" height="866" alt="Screenshot (170)" src="https://github.com/user-attachments/assets/9bd9d174-adc9-4339-9134-676dcd5df7f7" />
<img width="1423" height="871" alt="Screenshot (171)" src="https://github.com/user-attachments/assets/80bfdf28-b87c-4979-802a-7a1704101b69" />
<img width="1414" height="863" alt="Screenshot (172)" src="https://github.com/user-attachments/assets/5d59706b-3592-47a0-9f6b-40c47ae05f46" />
<img width="1428" height="889" alt="Screenshot (173)" src="https://github.com/user-attachments/assets/7ba30e90-cd5f-43d1-b3d4-d605511c54ed" />

## Key Insights
* Myocardial Infarction and Prenatal Initial Visit had the highest total claim costs, while “Admit to ICU” incurred the highest base cost.
* Periodic reevaluation and management of healthy individuals had the longest encounter durations, while Renal Dialysis dominated in procedure-level length of stay.
* The youth age group had the longest average stay, indicating higher hospitalization or treatment needs among younger adults.
* Total and base claim costs fluctuated over the years, with noticeable peaks around 2015 and slight declines afterward.
* Longer stays are associated with higher total claim costs, though most encounters are of short duration.
* Medicare recorded the highest insurance coverage among payers.

## Recommendations
* Stakeholder: Hospital Management (Medical Director)
* Recommendation: Review cost structures for these high-cost procedures to identify opportunities for cost optimization, better resource allocation, and preventive strategies that can reduce expensive admissions

* Stakeholder: Clinical and Medical Teams
* Recommendation: Streamline evaluation processes and dialysis scheduling to improve patient flow, reduce waiting time, and optimize bed utilization.

* Stakeholder: Health Information Officers & Clinical Teams
* Recommendation: Investigate causes of longer stays (e.g., lifestyle, chronic conditions) and implement targeted wellness or preventive health programs for younger adults.

* Stakeholder: Hospital Management & Health Insurance Providers
* Recommendation: Analyze cost fluctuations to uncover root causes (policy changes, resource use, patient load) and implement strategies for stable budgeting and claim management.

* Stakeholder: Hospital Management & Clinical Teams
* Recommendation: Adopt early discharge planning, reinforce post-discharge monitoring, and implement case management systems to reduce avoidable prolonged stays.

* Stakeholder: Hospital Management & Health Insurance Providers
* Recommendation: Strengthen partnerships with Medicare while also engaging other insurers to expand patient access and diversify revenue.

## Conclusion
The recommendations emphasize cost control, operational efficiency, patient-centered care, and data-driven planning. By optimizing high-cost procedures, improving patient flow, addressing long stays among younger patients, and balancing insurance partnerships, the hospital can achieve better financial sustainability, enhanced patient outcomes, and improved overall efficiency.

## Contact Information
* LinkedIn: https://www.linkedin.com/in/estheraderonke
* Email: aladeloyeesther616@gmail.com
