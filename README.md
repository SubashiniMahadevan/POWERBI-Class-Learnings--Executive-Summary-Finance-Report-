# POWERBI-Class-Learnings--Executive-Summary-Finance-Report-

# Sales Analysis Report

## Executive Summary
This PowerBI report provides insights into the company's latest sales figures. The executive summary includes:

1. **Most Profitable Month and Year**: The analysis identifies the month and year with the highest profit.
2. **Top Performing Countries/Regions**: The report highlights the countries or regions where the company is seeing the most success.
3. **Recommendations for Investment**: Based on the analysis, recommendations are provided regarding which product and segment the company should continue to invest in.
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/c7b8715f-8682-4482-aff3-0229ad10967c)

<br>
<br>

## Data Sources
The analysis is based on data from the sample finance workbook provided by the company.

## Report Overview
The report consists of several visualizations and dashboards to effectively communicate the insights derived from the data. Here's an overview of what the final report includes:

1. **Profit Analysis by Month and Year**: Visualizations showcasing the profit trend over different months and years, highlighting the most profitable period.
2. **Geographical Performance**: Maps and charts illustrating sales performance by country or region, helping to identify areas of success.
3. **Product and Segment Analysis**: Visualizations presenting sales figures by product and segment, providing insights into which areas the company should focus on for investment.

This PowerBI report provides a comprehensive analysis of the company's sales figures, addressing the manager's requests for insights into profitability, geographical performance, and investment recommendations.

For any questions or further analysis, feel free to reach out to the project team.

## Get data:

- Download the Financial sample Excel workbook .

- Open Power BI Desktop.

- In the Data section of the Home ribbon, select Excel.

- Navigate to where you saved the sample workbook, and select Open.
  
## Prepare your data:

- Select the Financials table, and choose Transform Data

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/ae79e840-1b44-4024-b5c3-1910119d7408)
<br>
<br>

- Select the Units Sold column. On the Transform tab, select Data Type, then select Whole Number. Choose Replace current to change the column type.
  <br>

**The top data cleaning step users do most often is changing data types. In this case, the units sold are in decimal form. It doesn’t make sense to have 0.2 or 0.5 of a
unit sold, does it? So let’s change that to whole number.**

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/9419a11b-1bbc-4d0a-8a39-6e803e3e2cbc)
<br>
<br>

- Select the Segment column. We want to make the segments easier to see in the chart later, so let’s format the Segment column. On the Transform tab, select Format, then select UPPERCASE

  ![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/952c6d99-d2b1-4d65-86a8-6a0a0272e1e3)
  <br>
  <br>

  - Let's shorten the column name from Month Name to just Month. Double-click the Month Name column, and rename to just Month.
 
  ![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/3d7ecc80-f05a-4c41-a617-f33f36efc81f)
  <br>
  <br>

  - In the Product column, select the dropdown and clear the box next to Montana.
We know the Montana product was discontinued last month, so we want to filter this data from our report to avoid confusion
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/9eb6dd4e-1290-489d-ac0f-64d243ff2426)
<br>
<br>

- You see that each transformation has been added to the list under Query Settings in Applied Steps.
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/cf6949a3-7408-464f-bf13-3a310d0b2ac1)
<br>
<br>

- Back on the Home tab, select Close & Apply. Our data is almost ready for building a report.

**You see the Sigma symbol in the Fields list? Power BI has detected that those fields are numeric. Power BI also indicates the date field with a calendar symbol.**

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/f397ce0a-0187-4f4c-8465-41e190580d9e)
<br>
<br>

- Write an expression in DAX
Writing measures and creating tables in the DAX formula language is super powerful for data modeling. There's lots to learn about DAX in the Power BI documentation. For now,
let's write a basic expression and join two tables.

**On the Home ribbon, select New measur**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/91ddeccb-5206-47c4-9c08-69c57e1e3e60)
<br>
<br>

**Type this expression to add all the numbers in the Units Sold column.**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/0600bf0b-6b45-457a-a745-e9e52fb4a46a)
<br>
<br>

**Select the check mark to commit**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/d737bb7d-3e1a-4231-a5a1-6073ef13ba7b)
<br>
<br>

**Now select the Data view on the left**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/df5a6dba-0d20-4797-835f-c27fb2c84a6f)
<br>
<br>

**On the Home ribbon, select New table**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/64bfc6d0-48c3-4ea4-81b6-e8177a34e5a0)
<br>
<br>

**Type this expression to generate a Calendar table of all dates between January 1, 2013, and December 31, 2014.**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/77bbb24d-1599-4044-a075-3474cb9c99cd)
<br>
<br>

**Select the check mark to commit**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/2c8448ab-71ed-44ab-a3ed-14371b98e356)
<br>
<br>

**Now select Model view on the left.**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/ff2ff1a9-ec36-4d3a-9803-d4a3ee410594)
<br>
<br>

**Drag the Date field from the financials table to the Date field in the Calendar table
to join the tables, and create a relationship between them.**
<br>

![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/22234824-4897-4ea1-a2b6-eb7a2fd6d789)
<br>
<br>

## Build your report:
<br>

- Add a title.
- Create a line chart to see which month and year had the highest profit.
- Profit by Country/Region - Create a map to see which country/region had the highest profits.
- Sales by Product and Segment - Create a bar chart to determine which companies and segments to invest in.
- Year slicer - Date slicer using the original table.
<br>


**In summary, this report answers top questions:**

***1. Which month and year had the most profit?***
<br>

<p>December 2014</p>
<br>
  
***2.Which country/region is the company seeing the most success in?***
 <br>
 
<p>In Europe, specifically France and Germany.</p>
<br>

***3.Which product and segment should the company continue to invest in?***
<br>

<p>The company should continue to invest in the Paseo product and target the Small Business and Government segments.</p>

<br>
<br>


![image](https://github.com/SubashiniMahadevan/POWERBI-Class-Learnings--Executive-Summary-Finance-Report-/assets/168095179/e5fcc1ce-9777-478b-a50c-fed826873921)
<br>
<br>



















  
