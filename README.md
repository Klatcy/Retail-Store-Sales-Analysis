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

  
![Sales Data Pivot Table](https://github.com/user-attachments/assets/65095be0-760f-4e50-92f4-7aa5d8a7b8b6)

- The above pivot table shows the report of Total Sales by Product, Region and Month, Top 3 Sales by Product and Average Sales per Product.
  

![Sales Data Pivot Table 2](https://github.com/user-attachments/assets/d9b40220-c175-43d8-a0c3-94823f496ca2)

- The above pivot table shows the report of Average sales per Product, Total Revenue by Region, Total Monthly Sales for Year 2023 and 2024 and Percentage of Total Sale.



![Excel Sales visualization](https://github.com/user-attachments/assets/50322d02-2866-489b-9cd7-85504f646f20)

- In analysing the data sales, column chart, pie chart, bar chart and line was used to analyse the sales performance of the retail store.



  #### PowerBI Data Visualization


![Sales data visualization with year](https://github.com/user-attachments/assets/81b085a8-da8d-4bb3-9787-c491870e27f5)



![Sales data visualization without year](https://github.com/user-attachments/assets/cb4ec0dd-afb8-46c3-b4f8-fec31fd4ac90)


### Conclusion

#### Overall Sales Trend
- The total sales by product is 2,101,090 million. Shoe recorded the highest sale with a total of 613,380 thousand, which is  , while Socks with a total of 180,000 thousand which  is    of the total sales recorded the lowest sales generated.
  
- The region with the highest total sales is South with 927,820 thousand, while West with a total of 300,345 thousand recorded the lowest sale by region.

- The most productive month




### Recommendation
In the light of the analysis carried out, 
