# HR Workforce Analytics Dashboard

## Project Overview

This project focuses on analyzing employee workforce data to identify key factors affecting employee attrition, performance, satisfaction, and salary distribution. The dashboard provides HR teams and management with actionable insights to improve employee retention and workforce planning.

## Business Problem

Organizations often struggle to understand why employees leave and which factors contribute most to attrition. This dashboard helps answer critical HR questions such as:

* Which departments experience the highest attrition?
* Does overtime increase employee turnover?
* Which age groups are more likely to resign?
* How does salary impact employee retention?
* What is the relationship between employee satisfaction and performance?

## Tools Used

* Power BI
* DAX
* Power Query
* Data Modeling
* Data Visualization

## Dataset Information

The dataset contains employee information including:

* Employee ID
* Department
* Job Role
* Gender
* Age
* Monthly Income
* Attrition Status
* Performance Rating
* Job Satisfaction
* Work-Life Balance
* Overtime
* Years at Company
* Training Times Last Year

---

## Dashboard Pages

### 1. Executive Summary

#### Visualizations

* Total Employees by Department
* Gender Distribution
* Attrition Distribution
* Salary by Department 

### 2. Attrition Analysis

#### Key Questions Answered

* Which department has the highest attrition?
* Does overtime increase attrition?
* Which age group resigns the most?

#### Visualizations

* Attrition by Department
* Overtime vs Attrition
* Attrition by Age Group

### 3. Salary Analytics

#### Visualizations

* Salary Distribution
* Salary by Department
* Salary by Job Role
* Highest Paid Employees

#### Salary Segmentation

* Low
* Medium
* High
* Premium

#### Visualizations

* Performance by Department
* Satisfaction by Department
* Training vs Performance


### 5. Advanced Insights

#### Visualizations

* Experience vs Salary
* Overtime vs Satisfaction
* Attrition Heatmap (Department vs Job Role)


## DAX Measures Created

```DAX
Total Employees = COUNT(EmployeeID)

```DAX
Attrition Count =
CALCULATE(
    COUNT(EmployeeID),
    Attrition = "Yes"
)

```DAX
Attrition Rate % =
DIVIDE([Attrition Count],[Total Employees],0)
```

```DAX
Average Salary =
AVERAGE(MonthlyIncome)
```

```DAX
Average Performance =
AVERAGE(PerformanceRating)
```

```DAX
Average Satisfaction =
AVERAGE(JobSatisfaction)
```

```DAX
Average Experience =
AVERAGE(YearsAtCompany)
```


## Key Insights

* Identified departments with the highest employee turnover.
* Evaluated the impact of overtime on attrition.
* Analyzed salary distribution across departments and job roles.
* Examined employee satisfaction and work-life balance trends.
* Explored relationships between experience, salary, and performance.


## Interactive Filters (Slicers)

The dashboard includes the following slicers:

* Department
* Gender
* Age Group
* Job Role
* Attrition

---

## Deliverables

### Power BI File

HR Workforce Analytics Dashboard.pbix

### Dashboard Screenshots

* Executive Summary Dashboard
* Attrition Analysis Dashboard
* Salary Analytics Dashboard
* Employee Performance Dashboard
* Advanced Insights Dashboard

---

## Author

**Suffian Khan**

Aspiring Data Analyst skilled in Power BI, SQL

