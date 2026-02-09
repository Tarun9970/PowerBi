Hospital Patient Analytics Dashboard

Data set:
Synthetic data covering roughly one thousand patients from Massachusetts General Hospital between 2011 and 2022.
The data includes patient demographics, insurance and payer details, hospital encounters, admissions, readmissions, procedures, costs, and coverage.

Project goal:
Build a clean and structured Power BI report that shows operational and clinical performance across encounters, admissions, readmissions, procedures, and mortality.
The focus is on demonstrating strong data handling, modeling, and analytical logic rather than just visuals.

Objectives:
Track encounters, admissions, and readmissions over time
Measure length of stay and admission behavior
Analyze visit costs and insurance coverage
Understand procedure volume, cost, and coverage
Highlight readmission and mortality patterns

Analysis pipeline:
Explore and understand patient, encounter, and procedure data → Prepare and enrich data for analysis → Build a star schema data model → Apply business logic for admissions, readmissions, and mortality → Create measures and KPIs for reporting → Design dashboards for non admissions, admissions and procedures

Core analysis and data preparation:
Encounters were split into non admissions and admissions based on length of stay rather than encounter class alone.
Admissions were further classified into initial admissions and readmissions using previous discharge dates and a thirty day window.
Procedures were aggregated at encounter level to support cost and volume analysis.
Patient level attributes such as age, age group, and mortality indicators were derived and linked to encounters.

Key steps:

Power Query:
Cleaned and standardized date and time fields
Merged patient and encounter data to calculate age at encounter
Created age groups and length of stay categories
Grouped procedures to calculate total procedure cost per encounter
Built supporting dimension tables such as date, age group, and encounter class

Power BI Desktop:
Built calculated columns using SWITCH and logical conditions
Identified admissions, initial admissions, and readmissions
Calculated length of stay metrics and bins
Created mortality indicators based on patient death dates
Built measures for rates, averages, trends, and KPIs using DAX

Data model:
A star schema was used with encounters as the main fact table.
Patients, payers, organizations, dates, and supporting dimensions were connected using one to many relationships.
The procedures table was linked only to encounters to ensure accurate aggregation and avoid ambiguity.

Outcome:
The final dashboard provides a clear view of hospital utilization, patient behavior, costs, coverage, readmissions, and mortality trends.
The project emphasizes realistic healthcare logic, structured modeling, and practical Power BI techniques suitable for intermediate level analytics roles.

