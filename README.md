# AdventureWorks Executive Summary Sales Repor

## Project Overview
This project focuses on building a dimensional model and dashboard of already clean data, reporting recent sales at AdventureWorks. It utilises brilliant visuals and data transformation using a simple DAX formla to create important sales column to create report that serves to provide an executive summary answering these questions:
- Which day had the most sales in February 2019?
- Which country/region is the company seeing the most success in?
- Which product category and reseller business types should the company continue to invest in?

This project has been published to Power BI service from Power BI desktop and can be accessed [here](https://app.powerbi.com/groups/me/reports/23bffe65-b4cb-4b69-9691-e11a8ac7f6ff/ReportSection?experience=power-bi)

## Data Transformation
- The worksheet with entities identified as relevant to the report under go transformation in Power BI before is loaded and modelled.
- The data type of each column assigned is verified and changed when necessary and changes made to wueries are applied. 



## Power BI Model
A star schema model was created to express relationship between sales data fields collected from different departments at the company.This promotes better understanding of the data.
The Sales field is the central concept(fact) surrounded by other several concepts with keys contained in fact, adding dimension.
Active and inactive relationships are created.
Heirachies were created and tables renamed.



## DAX Measure
Calculation includes inactive query from model and USERRELATIONSHIP function is used.
CALCULATE function is used to calculate the total sales amount by due date on the sales order instead of the default order date.



## Power BI Visualisation
In report view:
- A line plot of Sales amount by date.
- A map plot of order quantity by region.
- A column chart to show sum of sales by month with the month of february highlighted. This is also used as a Tool tip.
- A matrix showing sales amount by category of product.
- A filter for fiscal year.



## Findings
Based on the analysis, the following key determinants were identified:

The most sales in the month of february for the year 2019 was approximately 2.9 million dollars.
North America is the region-country with most sales in the bikes category. This is followed by components.
Australia was the next region-country with high sales and orders following the same product category order.
The reseller business type the company should keep investing in are warehouses and value added resellers.



## Data Source & License 
[Excel workbook](https://github.com/microsoft/powerbi-desktop-samples/blob/main/AdventureWorks%20Sales%20Sample/AdventureWorks%20Sales.xlsx)
This project is licensed under the MicroSoft Power BI Cloud skills challenge .