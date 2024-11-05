 # LITA_Project_2024

### Project Title: Retail Store Sales Analysis
---
### Introduction
The world of business thrives on data-driven decisions, and the ability to harness the power of data is essential. In this project, i embark on an exciting journey to analyze sales data, uncover trends, and reveal valuable insights that will drive strategic decision-making. The goal is to extract information from a retail store sales dataset, in order to provide a roadmap for the optimization of sales strategies in achieving sustainable growth.
---
## Project Overview
This Data Analysis aims at generating insight into the sales perforrmances of a Retail store over the past years. In analyzing the sales data, i seek to extract necessary information from the sales dataset, to provide valuable insights that can guide decision-making process across various aspects of the business. These insights include the identification of sales per product, sales per month, sales per region,  best-selling products, top revenue-generating region among others. This will enable us to tell compelling stories around our data from the insight gotten, to know the best performance from our data and also to enable  the business make informed decisions to optimize operations, enhance marketing efforts, and maximize revenue. 
---
###  Data Sources
Data Sources
The primary source of the Data used here is Sales Data.Csv. This is an open source data that an be freely downloaded from an open source online such as kaggle or any other data repository site.
---
### About the Dataset
The dataset has sales data from 2023 to 2024. It consists originally of 7 columns which was modified further for the purpose of the analysis;

- Order_id: Unique identifier for each order placed by a customer

- Customer_id: Unique identifier of each customer

- Product: Products sold by the store

- Region : Region of each customers

- Order_date: Date the order was placed
 
- Quantity: Quantity ordered for each product

- Price Each: Price of each product
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
EDA involved the exploring of the Data to answer some questions about the Data in order to gain insights.
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
This is where i include some basic lines of code or queries or even some of the DAX functions used during the analysis; 
```SQL
Select* from [dbo].[Sales Data]

```
- To Retrieve Total Sales for each Product category
```SQL
Select Product, sum (Total_Sales) as Sales_Per_State from [dbo].[Sales Data]
GROUP By Product
```
- Number Of Sales Transaction in each Region
```SQL
Select Region,sum (Total_Sales) as Sales_Transaction from [dbo].[Sales Data]
GROUP By Region
 ```
 - Highest Selling Product By Total Sales Value
```SQL
Select Product, sum (Total_Sales) as Total_Sales from [dbo].[Sales Data]
GROUP By Product
Order By Total_Sales Desc
```
- Total Revenue By Product
```SQL
Select Product, sum (Revenue) as Total_Revenue from [dbo].[Sales Data]
GROUP By Product
```







