## Project Overview

This project uses Microsoft Excel to clean, transform, combine, and analyze healthcare data. Information from customer, medical examination, and hospitalization tables is brought together into a consolidated Healthcare sheet for analysis.

The project demonstrates practical skills in data preparation, Excel formulas, lookup functions, PivotTables, and charts.

## Objectives

- Clean missing and inconsistent values.
- Split customer names into separate fields.
- Standardize healthcare categories and convert surgery counts to numeric values.
- Create weight-status and diabetes-status categories.
- Calculate date of birth and age.
- Combine information from multiple tables using Customer ID.
- Analyze healthcare measures and communicate findings with charts.

## Data Preparation

The data-cleaning and transformation steps include:

- Replacing 
?
 entries with blanks before analysis.
- Filling missing months with 
Sep
.
- Filling missing years with the rounded average year.
- Replacing missing smoker and hospital/city tier values with the most frequent valid category.
- Marking unavailable State IDs as 
Unknown
.
- Splitting customer names into title, first name, and last name.
- Converting major-surgery labels to numeric values where the meaning is clear.
- Standardizing Heart Issues and smoker categories.
- Formatting charges as currency.

## Derived Fields

The project adds the following fields:

- Weight Status: Based on BMI.
  - Underweight: BMI below 18.5
  - Normal Weight: BMI from 18.5 to below 25
  - Overweight: BMI from 25 to below 30
  - Obesity: BMI of 30 or above
- Diabetes Status: Based on HbA1C.
  - Normal: HbA1C below 5.7
  - Prediabetes: HbA1C from 5.7 to below 6.5
  - Diabetes: HbA1C of 6.5 or above
- Date of Birth: Created from the year, month, and date fields.
- Age: Calculated as of 8 June 2023.

## Combined Healthcare Sheet

The final Healthcare sheet combines relevant data using Customer ID and includes fields such as:


Customer ID
, 
First Name
, 
BMI
, 
HBA1C
, 
Heart Issues
, 
Any Transplants
, 
Cancer history
, 
NumberOfMajorSurgeries
, 
smoker
, 
Weight Status
, 
Diabetes Status
, 
Date of Birth
, 
charges
, 
Hospital tier
, 
City tier
, 
State ID
, and 
Age
.

## Analysis and Visualizations

PivotTables and charts are used to explore relationships between:

- Smoking status and cancer history.
- Transplant history, number of major surgeries, and average HbA1C.
- Weight status, diabetes status, and healthcare charges.

## Tools

- Microsoft Excel
- Excel Tables and formulas
- XLOOKUP or VLOOKUP
- PivotTables
- Excel charts

## How to Use

1. Download or clone this repository.
2. Open the Excel workbook in Microsoft Excel.
3. Review the cleaned data and combined Healthcare sheet.
4. Use the PivotTables and charts to explore the analyses.

## Notes

- Missing or ambiguous values should not be interpreted as confirmed negative results.
- Customer ID is used to combine records, so IDs should be checked for duplicates before joining tables.
- This project is for educational and analytical purposes and is not medical advice.
