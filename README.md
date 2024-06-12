# Business-Insights-360----Power-BI

## Project Overview
AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

## Tech stacks
- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## PowerBI techniques Learnt
- What are all the questions should be asked before staring the project
- Creating calculated columns
- Creating measure using DAX language
- Data modeling
- Using divide function to prevent zero division errors
- Creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Data validation techniques
- PowerBi services

## Business related terms
- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Dataset Understanding.
Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

- Dimension table : It will have the static data like details of customer and products

- Fact table : It will have the data about the transactions

- gdb041:
    - dim_customer
        -  27 distinct markets (ex India, USA, spain)
        -  75 distinct customers thorough out the market
        -  2 types of platforms
            - Brick & Motors - Physical/offline store
            -  E-commerce - Online Store (Amazon, flipkart)
        - Three channels
          - Retailer
          - Direct
          - Distributors
    - dim_market
      - 27 distinct markets (ex India, USA, spain)
      - 7 sub-zones
      - 4 regions
        - APAC
        - EU
        - nan
        - LATAM
    - dim_product
      - Divisions
        - P & A
          - Peripherals
          - Accessories
        - PC
          - Notebook
          - Desktop
        - N & S
          - Networking
          - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
      - This table is used to forecast the customer’s need in advance, which can help in
        - Higher customer satisfaction
        - Reduced cost in warehouses for storage purpose
      - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
      - All the date of the month will be replaced by the start date of the month
      - It will have all the column names and in the end it will have the forecast quantity need of the customer
    - fact_sales_monthly
      - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
  - gdb056
      - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
      - gross_price
        - Has the details of gross prices with product code
      - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
      - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer with year
      - Post_invoice_deductions
        - Post invoice deductions and other deductions details
          
## Data Model
- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the over all performance of the report.
- Following Good practices of data modeling is must. Refer this page to get to know the good practices Blog
- In this project, we have followed Snowfall data modeling method.

![image](https://github.com/Sankari0299/Business-Insights-360----Power-BI/assets/122591357/5e71d06f-26b7-468b-bf06-f93d72481528)


## Dashboard Designing
## Home view
  - In Home view, all the views button will be available. User will land on specific view page by clicking the button
    - Info
    - Finance View
    - Sales View
    - Marketing View
    - Supply chain View
    - Executive View
    - Products
    - Support

  ## Home 
  
![Screenshot 2024-06-11 215307](https://github.com/Sankari0299/Business-Insights-360----Power-BI/assets/122591357/689b6992-dc93-4db4-954f-0b3a20b9986f)

## Finance View

![Screenshot 2024-06-11 215336](https://github.com/Sankari0299/Business-Insights-360----Power-BI/assets/122591357/3fd532e2-9285-421d-9cc1-592db08b96e1)

## Sales View

![Screenshot 2024-06-11 215347](https://github.com/Sankari0299/Business-Insights-360----Power-BI/assets/122591357/b206e6f3-b3be-49ea-b144-984a2d8fa0ac)

## Marketing View

![Screenshot 2024-06-11 215402](https://github.com/Sankari0299/Business-Insights-360----Power-BI/assets/122591357/b0bcd156-9408-4ab2-bdc1-d7e3b8c458fe)

## Supply Chain View

![Screenshot 2024-06-11 215414](https://github.com/Sankari0299/Business-Insights-360----Power-BI/assets/122591357/a64561af-c814-42ae-9559-4ff6ec78e706)

## Project Outcome
By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
