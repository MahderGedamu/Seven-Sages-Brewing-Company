# Seven-Sages-Brewing-Company Dashboard
### Overview
Project 1: Data Modeling and Reporting with Power BI
Completed: November 2024
Nanodegree Program: Data Analysis and Visualization with Microsoft Power BI (Udacity)

In this first project of the Nanodegree program, we worked on preparing and modeling data using Microsoft Power BI. The project centered around a fictional company called Seven Sages Brewing Company and involved building a comprehensive Power BI data model and report that brings together information from various departments within the company to efficiently evaluate the performance of its beer products across various dimensions such as sales volume, profitability, product categories, and distribution channels.
Currently, the company lacks a centralized and visual way to assess which beers are top performers in terms of revenue and profit, and which ones may be underperforming or operating at a loss.

The primary objective was to enable the company's CFO to easily analyze beer sales performance and identify which products are generating the highest profitability. Using the provided data sources, we were tasked with recreating a pre-defined report layout, ensuring that the visualizations and metrics aligned with the company's analytical goals.

This project emphasized core Power BI skills, including data transformation, relationship modeling, and building insightful dashboards to support strategic decision-making.
To address this, a Power BI dashboard has been developed leveraging a robust data model that integrates sales transactions, production costs, and product attributes.
This solution empowers the CFO to:

-Quickly identify the best-selling beers and analyze sales trends over time.

-Evaluate profitability by product, category, and region to ensure every product is contributing positively to the company’s bottom line.

-Detect loss-making or low-margin beers to support strategic decisions such as pricing adjustments, discontinuation, or marketing focus.

-Drill down into detailed KPIs such as cost of goods sold (COGS), profit margins, and unit economics.

-Visualize performance comparisons across time periods, locations, or customer segments.

-This data-driven approach enhances financial oversight, supports more accurate forecasting, and contributes to smarter business decisions that align with the company’s growth and efficiency goals.

### Steps followed/ ETL

  Step 1 : Using "Get Data" accessed the necessary data sources and pulled them into Power BI.
             The source material for this project can be found under the folder called “source files”.

             Promotional document: The sales department has provided a promotional document that lists all the company’s current offerings, ratings, and servings sizes.

             Purchases: An operations assistant has provided data on purchases, in the form of multiple Excel spreadsheets

             Customer records: IT has provided customer records. They had to download these separately, but they have assured us that they are up to date.

             Metrics documentation: The CFO has provided her metrics documentation that she’s been compiling on sales, costs, and servings (per
             
 Step 2 : Using power query editor & Structured, Combined, and Cleaned the Data.
           Data Cleanup:
           
           Promoted first rows to headers as needed

           Reviewed data types for each field to ensure that they are identified correctly

           Renamed any ambiguous queries so that they can be easily identified during data modeling

           Renamed any unclear columns so you can easily find and use them

           Removed any or all blank rows

           Deleted unnecessary columns

          Corrected any obvious typos that will impact report results

          Combining Data:
          
           Merged dimension tables with a 1-to-1 relationship

           Merged CFO Metrics Tracker and SSBC Product Offerings to create the Product table

           Combined Sales files under the “Monthly Sales Logs” folder into one Sales table. (Files include columns of the name.)

### Date Table Creation

Created a dynamic date table that starts at the beginning of the calendar year of the earliest Sales year and ends at the end of the calendar year for the latest year on the Sales table.

This continuous table includes the following columns:

•	Calendar month name and number

•	Calendar year

•	Fiscal period

•	Fiscal year

•	Fiscal quarter -Quarter - FY (e.g., Q1 - FY2021)

Seven Sages' Fiscal year begins on October 1st and runs until September 30th.

![Image](https://github.com/user-attachments/assets/bfcb817d-f39f-4144-9b86-df2618d9ee7e)

## Fact Table

Sales

## Dimension Tables

Products

Customers

Calendar

Exchange Rates

## Measures
Total Sales ($USD)

Cost of Sales ($USD)

Gross Profit Margin (%)

Sales ($CAD)

Unit Sales by Product (%, USD)

Gross Profit by Product (%,USD)

 Step 3 : Built Relationships Between Tables. Built a relationship from each dimension to the relevant key on the fact table with a one-to-many relationship.
 
 Step 4 : Measures Created. To satisfy the CFO's requirements, calculated the Sales, Cost of Sales and Gross Profit Margin in two different currencies.

 # Report
 ## Tab #1

 ![Image](https://github.com/user-attachments/assets/1b14338d-9ba0-463d-a5dc-8e12cec745a3)

 Sales and GPM: This tab summarizes the sales by customer and customer type across quarters.

  ## Tab #2
  ![Image](https://github.com/user-attachments/assets/74f5f285-a52e-45a4-bd27-f42316a1cddb)

  Gross Profit and Unit Sales: This tab would simply summarize the percentages of gross profit and unit sales by product.

   ## Tab #3
   ![Image](https://github.com/user-attachments/assets/29c58d45-66ae-4231-98a8-64011594ab17)

   This tab shows what product type is most profitable per serving for SSBC.

   ## Tab #4
   ![Image](https://github.com/user-attachments/assets/78fe66ff-be96-43f6-98c5-323920289cc0)
 
      Seasonality, reviews the trends over the course of the calendar year.

        

