# HR-Data-Analytics-Dashboard(Excel,Tableau)
# HR Analytics Dashboard

## Overview
This project aims to analyze employee attrition within a company using an interactive dashboard built with Excel and Tableau. By examining various factors such as age, experience, and income, the dashboard provides insights into trends and patterns related to employee departures.

## Problem Statement
The HR Director has observed an increase in employee attrition and seeks to identify trends or factors contributing to this issue. The project focuses on:
- Calculating the attrition rate.
- Analyzing the impact of age, years at the company, and income on employee retention.

## Getting Started
To replicate the dashboard, follow these steps:

### Data Loading
- Download the dataset provided in CSV format.
- Open Tableau and select "Text/CSV" on the landing page in the data source section.
- Locate and load the dataset.

## Data Visualization Steps
### Sheet 1: Age-Wise Employee Count
- Create a new column grouping ages into the following categories: 18-25, 26-35, 36-45, 46-55, 56-60.
- Create a stacked bar chart to show employee counts by age group, using the attrition column for color differentiation.

### Sheet 2: Average Monthly Income by Age
- Create a dual bar chart to display the average monthly income of each age group.
- Use Level of Detail (LOD) calculations for average income per age group and overall average income.

### Sheet 3: Employee Count by Income
- Create a histogram to show monthly income distribution with a bin size of 2000, using the attrition column to differentiate the data.

### Sheet 4: Employee Count by Experience
- Develop a bar chart indicating the employee count based on the number of years worked in the company, again using the attrition column for color differentiation.

### Headline Cards
- Add headline cards to display key metrics:
  - Total Employee Count
  - Employee Leaving Rate (calculated using attrition data)
  - Job Satisfaction (Average)
  - Average Monthly Income (Average)

### Dashboard Assembly
- Set the dashboard size to 1300 x 900.
- Drag and drop the sheets, adjusting sizes as desired.
- Add filters based on attrition to customize visualizations across the dashboard.

## Flowchart
Refer to the flowchart diagrams for a visual representation of the data ingestion, processing, visualization, and dashboarding processes.
<img width="3708" height="3820" alt="Data Analysis Flowchart" src="https://github.com/user-attachments/assets/96f9fe07-875a-4701-b998-fa50f8e2b8ea" />
<img width="2884" height="1516" alt="HR Analysis Flowchart" src="https://github.com/user-attachments/assets/9bf2245b-aadc-4719-9d43-311622ff1f3a" />


## Conclusion
This dashboard provides valuable insights into employee attrition, allowing HR leaders to understand underlying trends and factors contributing to employee retention. It can be further enhanced by exploring additional variables or creating new visualizations.


## Dashboard
<img width="1540" height="863" alt="5 Dashboard" src="https://github.com/user-attachments/assets/8217bd5a-7904-4051-9322-2ee90c7de8fc" />
