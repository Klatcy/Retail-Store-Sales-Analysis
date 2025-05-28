 ### LITA_PROJECT 2024

### Project Title: Retail Store Sales Analysis
### Table of Contents

- [Introduction](#introduction)

- [Project Overview](#project-overview)

- [Data Sources](#data-sources)

- [About the Dataset](#about-the-dataset)

- [Tools Used](#tools-used)

- [Data Cleaning and Preparations](#data-cleaning-and-preparations)

- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis)

- [Data Analysis](#data-analysis)

- [Data Visualization](#data-visualization)
  
---
### Introduction
 The world of business thrives on data-driven decisions, and the ability to harness the power of data is essential. In this project, i embark on an exciting journey to analyze Retail Store sales data to uncover trends, and reveal valuable insights that will drive strategic decision-making. In other words, the goal is to extract information from the sales dataset, in order to provide a roadmap for the optimization of sales strategies in achieving sustainable growth.
 
 --- 
### Project Overview
This Data Analysis aims at generating insight into the sales perforrmances of a Retail store over the past years. In analyzing the sales data, i seek to extract necessary information from the sales dataset, to provide valuable insights that can guide decision-making process across various aspects of the business. These insights include the identification of sales per product, sales per month, sales per region,  best-selling products, top revenue-generating region among others. This will enable us to tell compelling stories around the data from the insight gotten, to know the best performance from our data and also to enable  the business make informed decisions to optimize operations, enhance marketing efforts, and maximize revenue.

---
 ###  Data Sources
The primary source of the Data used here is Sales Data.Csv. This is an open source data that an be freely downloaded from an open source online such as kaggle or any other data repository site.
 
---
### About the Dataset
The dataset has sales data from 2023 to 2024. It consists originally of 7 columns which was modified further for the purpose of the analysis;

- OrderID: Unique identifier for each order placed by a customer

- CustomerID: Unique identifier of each customer

- Product: Products sold by the store

- Region : Region of each customers

- OrderDate: Date the order was placed
 
- Quantity: Quantity ordered for each product

- Price Each: Price of each product
  
- Total Sales:Total sales gotten for each product
  
- Revenue: Revenue generated from the product sold
  
---
### Tools Used
- Microsoft Excel {Download Here}{https://www.microsoft.com}
  1. For Data Cleaning, 
  2. For Analysis
  3. For Data Visualization

 - Structured Query Language {SQL] for Quering of Data
  
- PowerBI for Dynamic and Interactive Data Visualization.

- GitHub for Portfolio Building

---
### Data Cleaning and Preparations.
In the initial phase of the Data cleaning and preparations, the following actions were performed; 
 1. Data Loading and Inspection
 2. Handling Missing Variables
 3. Data Cleaning and Formatting

---
### Exploratory Data Analysis (EDA)
EDA involved the exploration of Data to answer some questions about the Data in order to gain insights. The questions are categorized into two, which are: Sales Analysis and Product Analysis.
#### Sales Analysis
- What is the total sales per product ? 
- What is the total sales per month?
- What is the total sales per region?
- What is the revenue by region?
#### Product Analysis
- Which product sold the most?
- Which product are top sellers?
- What is the average sales per product?

---
### Data Analysis
This is where i include some basic lines of code or queries or even some of the DAX functions used during the analysis.These include
- SQL Queries
```SQL
SELECT* FROM [dbo].[Sales Data]
```
- To Retrieve Total Sales for each Product category
```SQL
SELECT Product, SUM (Total_Sales) as Sales_Per_State FROM [dbo].[Sales Data]
GROUP By Product
```
- To Find the Number of Sales Transaction in each Region
```SQL
SELECT Region, SUM(Total_Sales) as Sales_Transaction FROM [dbo].[Sales Data]
GROUP By Region
 ```
 - To Find the Highest Selling Product by Total Sales Value
```SQL
SELECT Product, SUM (Total_Sales) as Total_Sales FROM [dbo].[Sales Data]
GROUP By Product
Order By Total_Sales DESC
```
- To Calculate Total Revenue by Product
```SQL
SELECT Product, SUM (Revenue) as Total_Revenue FROM [dbo].[Sales Data]
GROUP By Product
```
- To Order Month Column
```SQL
ALTER TABLE [dbo].[Sales Data]
ADD Order_Month Nvarchar(50)
```
```SQL
UPDATE [dbo].[Sales Data]
SET Order_Month = DATENAME(month, OrderDate)
```
```SQL
ALTER TABLE [dbo].[Sales Data]
ADD Order_Year INT
```
```SQL
Update [dbo].[Sales Data]
SET Order_Year = Year (OrderDate)
```
- Monthly Sales For The Current Year
```SQL
SELECT  Order_Month, SUM (Total_Sales) AS Monthly_Sales FROM [dbo].[Sales Data]
WHERE Order_Year=2024
GROUP By Order_Month
```
- PowerBI DAX functions
 
 1.To count total customers in each region.
   Conditional column 
   
If Region = North then 1,
If Region = South then 2,
If Region = West then 3.
If Region = East then 4,
Otherwise, 5.

---
### Data Visualization

#### Microsoft Excel Data Visualization

  
![Sales Pivot Table 1](https://github.com/user-attachments/assets/68035b42-bdbb-49d1-b1cb-d2fda9fa5175)



- The above pivot table shows the report of Total Sales by Product, Region and Month, Top 3 Sales by Product and Average Sales per Product


![Sales Pivot Table 2](https://github.com/user-attachments/assets/54e36e13-562d-412a-ac11-de161de954d0)


- The above pivot table shows the report of Average sales per Product, Total Revenue by Region, Total Monthly Sales for Year 2023 and 2024 and Percentage of Total Sale.

  
 ![Excel Sales Visual](https://github.com/user-attachments/assets/57bdc445-703f-4051-b2b5-1bc4a9799025)
 

- In analysing the data sales, column chart, pie chart, bar chart and line was used to analyse the sales performance of the retail store.



  #### PowerBI Data Visualization


![Sales Visual - PowerBI](https://github.com/user-attachments/assets/09978cb3-dfbf-4285-b218-1ed18e453977)





### Conclusion

#### Overall Sales Trend
- The total sales by product is 2,101,090M. Shoe recorded the highest sale with a total of 613,380 thousand, while Socks with a total of 180,000K recorded the lowest sales generated.
  
- The region with the highest total sales is South with 927,820 thousand, while West with a total of 300,345 thousand recorded the lowest sale by region.

- The most productive month is February with a total sales of 546,300K. While has the least sale from January 2023 to August 2024.

- The top performing product is Shoes which generated total sale of 613,380K, while the least performing product is Socks which generated a total sale of of180,785K.

- The Average Sales by Product is 211.78

- The Total Revenue is 2,101,090K

- The total number of customers in all the region is 9921. North region has 


### Recommendation
In the light of the analysis carried out, the following recommendations are made:

## Product-wise Recommendations:

 - Focus on Shoes: Continue investing in Shoes, as they're top-selling products.
-Improve Socks Sales: Analyze reasons for low Socks sales and consider:
    - Marketing campaigns
    - Product redesign
    - Promotions

## Region-wise Recommendations:

- Expand South Region Strategy: Replicate successful strategies from South region in other regions.
- Boost West Region Sales: Identify challenges in West region and develop targeted strategies.

##Monthly Sales Optimization

- Analyze February's Success: Identify factors contributing to February's high sales and leverage them in other months.
- Improve January Sales: Develop strategies to boost sales in January.

## General Recommendations:

- Data-driven Decision Making: Use data insights to inform product, marketing, and regional strategies.
- Customer Engagement: With 9921 customers, focus on enhancing customer experience and loyalty.

## Actionable Steps:

- Conduct market research to understand customer preferences.
- Develop targeted marketing campaigns for Socks and West region.
- Analyze product pricing and adjust accordingly.

These recommendations can help optimize sales, revenue, and customer engagement.
