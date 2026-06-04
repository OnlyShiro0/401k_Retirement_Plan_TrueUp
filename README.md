OVERVIEW

This project automates the process of identifying eligible employees for a 401(k) True-Up calculation and recalculates employer matching contributions based on annual compensation and employee deferral rates.

Using Python and Pandas, the workflow cleans raw employee census data, applies plan eligibility rules, converts financial fields into analytical formats, and prepares the dataset for year-end retirement plan reconciliation.

BUSINESS PROBLEM

Many organizations calculate employer matching contributions on a payroll-by-payroll basis. As a result, employees who front-load or vary their contributions throughout the year may not receive the full employer match they are entitled to under an annualized calculation.

This project helps identify:

Employees eligible for True-Up calculations
Employees who may have received less than the maximum employer match
Additional employer contributions required for compliance with plan provisions
Dataset

1. Data Validation & Exploration
Load employee census data
Inspect dataset structure
Identify missing values
Validate data types

3. Data Cleaning
Standardize date columns
Correct future birth dates caused by two-digit year formatting
Handle missing and invalid values
Rename columns for readability

4. Employee Eligibility Filtering
Employees are considered eligible only if they meet all plan requirements:

Entry date before January 1, 2023
Employed on the last day of the plan year
Worked at least 1,000 hours
Full-time employee status

4. Financial Data Processing
Convert currency fields into numeric values
Remove formatting characters ($, commas)
Apply IRS compensation limits
Calculate total employee deferrals

5. True-Up Preparation
Calculate annual deferral rates
Determine compensation subject to matching
Prepare final dataset for employer match reconciliation
Technologies Used
Python
Pandas
Jupyter Notebook / Google Colab

Skills Demonstrated
Data Cleaning
Data Validation
ETL Processes
Financial Data Analysis
Retirement Plan Analytics
Business Rule Implementation
Pandas Data Manipulation
Eligibility Calculations
401(k) True-Up Analysis

Example Output

The final dataset includes:

Employee	Eligible Compensation	Deferrals	Deferral Rate
Employee A	$82,460	$17,219	20.88%
Employee B	$71,936	$3,925	5.46%
Employee C	$132,735	$20,500	15.44%

This output can be used as the foundation for calculating year-end True-Up contributions and validating employer match compliance.
