
# HR Analytics Dashboard - Power BI Project

## Introduction
This project involves creating a comprehensive HR analytics dashboard using Power BI. The dashboard provides key insights into various aspects of employee data, including demographics, performance, promotion eligibility, and retrenchment status. It is designed to help HR departments make informed, data-driven decisions.

## Problem Statement
Organizations often struggle with understanding workforce dynamics due to fragmented data and a lack of visual insights. This project addresses this challenge by consolidating HR data into a single, user-friendly dashboard. The goal is to provide HR teams with clear, actionable insights to improve workforce management, retention strategies, and overall employee satisfaction.

## Skills Demonstrated
- **Data Analysis**: Efficiently extracting, transforming, and analyzing HR data.
- **Power BI Visualization**: Crafting intuitive visualizations, including KPI cards, charts, and tables, for clear data interpretation.
- **DAX Calculations**: Utilizing DAX for dynamic calculations to ensure accurate insights across various metrics.
- **Data Cleaning and Transformation**: Using Power Query to clean and standardize raw data, making it ready for analysis.

## Data Transformation and Visualization
### Data Sources
- **HR Employee Data.xlsx**: Contains raw data about employees, including demographics, job roles, and performance ratings.
- **HR Analytics Data.xlsx**: Additional dataset providing further details on employee statuses.
- **HR Clean Table.xlsx**: The processed dataset, cleaned and standardized using Power Query.

### Data Transformation
The raw data underwent various cleaning processes, including:
- Standardizing fields and removing duplicates.
- Handling missing values.
- Creating calculated columns to facilitate better analysis.

### Visualizations
The dashboard is organized across three pages, each focusing on distinct analytical aspects:

#### Page 1: KPI Overview and Employee Distribution
- **KPIs in Cards**: Shows metrics for total employees, and counts/percentages for male, female, on-service, retrenched, due for promotion, and not due for promotion.
- **Donut Chart**: Employee distribution based on distance from the office.
- **Column Chart**: Employees segmented by job level.
- **Stacked Bar Chart**: Total employees by years of service.

#### Page 2: Performance and Satisfaction Insights
- **Column Chart**: Employees due for retrenchment and promotion, categorized by department.
- **Pie Chart**: Employee distribution by job satisfaction and overtime status.
- **Percentage Indicators**: Highlighting high and low performance ratings.
- **Table**: Breakdown of job roles by total employees, retrenchment, and promotion status.

#### Page 3: Employee-Specific Information
- **Retrenchment Table**: Lists names of employees marked for retrenchment.
- **Promotion Table**: Lists names of employees eligible for promotion.

## DAX Calculations
The following DAX measures were created to derive accurate insights:
- **% Female**: `DIVIDE([female],[Total Emp],0)`
- **% Male**: `DIVIDE([Male],[Total Emp],0)`
- **% High Rating**: `DIVIDE([High Rating],[Total Emp],0)`
- **% Low Rating**: `DIVIDE([Low Rating],[Total Emp],0)`
- **% Due for Promotion**: `DIVIDE([Due for Promotion],[Total Emp],0)`
- **% Not Due**: `DIVIDE([Not Due],[Total Emp],0)`
- **% On Service**: `DIVIDE([On Service],[Total Emp],0)`
- **% Retrench**: `DIVIDE([Retrench],[Total Emp],0)`

These measures, along with complex `IF` statements, ensure precise handling of various employee attributes and statuses.

## Conclusion
The HR Analytics Dashboard is a versatile tool designed to empower HR professionals with deeper insights into workforce management. With easy-to-read visuals and reliable data, it aids in strategic planning for promotions, retrenchment, and employee satisfaction initiatives.

