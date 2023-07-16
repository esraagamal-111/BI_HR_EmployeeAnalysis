# BI_HR_Analysis
Power_BI_in_HumanResources_Analysis 


# Power_BI_in_Sales_Analysis
Power_BI_in_Sales_Analysis 

![hr](cover.jpg)

## Introduction
This project is to display Human resources Analysis using POWER BI. The problem satatement is an imaginary case scenario I thought about after seeing the dataset.

## Problem Statement
Our client a leading multinational corporation has been experiencing some puzzling trends in their employee turnover rates they suspect that there may be hidden factors causing valuable employees to leave.
As data master it’s our job to dig deep into their HR data and uncover the truth.

Creating one a Human resource dynamic report which answer the following questions:
1. What is the gender breakdown of current employees in the company?
2. What is the race breakdown of current employees in the company? 
3. What is the age  distribution of the current employees in the company?
4. What is the percentage of employees works on Headquarter vs Remote?
5. What is the average length of employement who have been termenated?
6. How does the gender distribution vary across department and job titles?
7. what is the distribution of the job titles across the company?
8. Which department has the highest termination rate?
9. What is the employee distribution across the location state?
10. How has the company employees count changed over time based on hirdate and termination date?
11. What is the tenure distribution for each department?


## Data Sourcing
 the information was in one table:
- hr

Data was then locally extracted from Excel Workbook into Power BI for transformation, analysis and visualization.

## Data Transformation

Data cleaning was performed.
The table appeared to be clean.
The quality of each column is 100% with no error or nulls.
Below is a preview of the tables:

     


**HT Table**
![](hrtb.png)

For the HR Table, first rows were not headers and so resolved that by applying the "Use First row as header" action.
Change birthdate,hirdate,termdate to date date type
calculate age column.

## Data Model Design
The data required for this analysis are located in various tables.
Therfore, appropriate modelling is required.
A star Schema is designed with the Sales and Returns Table representing the fact table containing all redundant data, and to which other dimension tables are modelled or connected to, using the column that is common. Date Table was created in power query using list of max and min date from sales tables
Sales & Rturns Table has been modelled with:
- Date Table using the "Date"
- Product Table using "Productkey"
- Customers Tables via "CustomerKey"
- Date Tables via "Date"

![model](DataModelling.png)


## Data Aanalysis/ Visualization
Analysis was done using simple visuals since the tables have been perfectly modelled together.
Applied some Dax Function to get the required information

## Sales performance

![](Sales_Performance1.png)

#### Sales performance is improving since 2010 till 2013 years.
#### Protein is the best sales contributes about 64 million to net sales compared with Carps 6 million 

2012 Returns             |          2013 Returns
:--------------------------:|:------------------------:
![](Sales_Performance.png)         |         ![](Sales_Performance2.png)

####  Focus on 2013 vs 2012 we can easily find that:
 - Net Sales goes up to $31M compared with $25M in 2012.
 - Gross Margin goes up to $20M compared with $16M in 2012.
 - Sales return improved in 2013 (6.46%) by about 3.5% below return margin allowed (10%) comparing with 2012 (10.34%) by about 0.34% over return margin allowed.

We can then Right click on "Category Order details
Here I Check Protein Order details.

![](OrderDetails.png)

## Gross Margin Year over Year
This dashboard clear the Gross margin:
 1- Year over year by month.
 2- Year to date comparing same period last year.
 3- Year over year by Category and subcategory.

 Here I filtered on 2013 comapring by 2012
 
 ![](GrossMarginYoY.png)

 #### Gross Margin is $20M in 2013 compared with $16M in 2012 by about 27%.
 #### Clearly find that 2013 follows same trend on 2012 with growing in gross margin except on May and August trend goes up on 2013 while it was down on 2012.
 #### Unfortenatly Jackets gross margin and Vests decreased by (100%, 93%) respectively in 2013 comapring by 2012.

 
## Customers Cross Selling and Customers Purchase

![](CustomerCrossSelling.png)

Obective : Number of customers whose purchased two product together.

![](CustomerCrossSelling2.png)

#### Focus on Aminox Bcaa we can find that only 5 customers purchase this product and all of then had bought Pro Weight Gainer with it


## Conclusions/Recommendations
- Over all sales performance is doing will since 2010 till 2013.
- Studying How can increase categories sales by making Promotion offer when buying from protein category.
- Studying the cross selling of Aminox Bcaa and other products especially Pro Weight Gainer and make Promotion offers on Aminox Bcaa.
------

###### My goal is to provide value to the stakeholders and not just to build reports and dashboard. 

Thank you.

