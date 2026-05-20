# Excel Project: Bike Buyers

## Overview 
I analyze customers' demographics (Age, Genders, Income, Commute Distance,...) in relation to their decisions whether to buy bikes or not.

## Main Tasks
1. Data Cleaning
2. Pivot Tables & Charts
3. Interactive Dashboard

## Task 1: Data Cleaning
Below is the raw dataset.
![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/b5ac3b15ab167d575f9ba4654ed65e7b51cd66be/Screenshot%202026-05-21%20043704.png)

### Problems regarding raw dataset
- Marital status (M/S) and Gender (M/F) both have "M" as their unit of identification.
- Age is continuous variable, which is not suitable for grouping and analysis

### Create Table
I start with create a table, which allows smoother calculation and formatting.

### Change Marital Status and Gender abbreviation
Under the Martial Status column, the values should be Married or Single. Under the Gender Column, the values should be Male or Female.

![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/d3c9bd74dd33690308c20d50c0afca2f199fe2eb/Screenshot%202026-05-21%20024712.png)

Then it turns out:

![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/5714249a4cfdd51417b17144a7ab5a79d3ba5880/Screenshot%202026-05-21%20045648.png)

### Create Age Range using IF function
I breakdown the Age into 3 groups:
- <36 years old: Young Adult
- 36-60 years old: Middle Age
- Over 60 years old: Elderly
Function: =IFS([@Age]<36,"Young Adult", AND(35<[@Age],[@Age]<61),"Middle Age",[@Age]>60,"Elderly")

The new column called "Age Brackets" utilize this:

![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/f57d4931fba950737848cd44787fa0e84a782959/Screenshot%202026-05-21%20050216.png)

The whole data after cleaning:

![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/b627be67ad7eb2f6c44c6a923b635b01066bf762/Screenshot%202026-05-21%20050400.png)

## Task 2: Analyze & Visualize data using Pivot Table
I used Pivot Table to have an overview of the trends and relationships between variables.

![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/6483137643472ded3752ddd193ba98dcbca07b7a/Screenshot%202026-05-21%20050922.png)

## Task 3: Create Dashboard
My final step of visualization is to add slices

![image alt](https://github.com/kristineng/Excel-Project_Customer-Analysis_Bike-Buyers/blob/2d35e35217ae199ef3be1ce89587c141afe6365c/Screenshot%202026-05-21%20051234.png)

For further details, please visit the excel project file uploaded above.

Thank you!
