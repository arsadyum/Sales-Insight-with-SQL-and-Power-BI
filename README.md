# Sales-Insight-with-Power-BI
# The problem: The Client have lots of unleaned Excel/CSV file containing sales/marketing data which can not produce any business Iinsight to increase revenue and profit. 

## Porpose ( AIMS GRID Project management tool) 4 parts: To discover insight from the provided data which is invisible for team's decision making process and eliminate manuall process of data gathering and data cleaning

## Stakholders/Parties involved:  * Product Owner * Marketing Analytics Team * Data Engineering Team 

## What is the Project Aiming for : An Automatic Power BI Dashboard offering quick insights on data to support decision making process. 

## Success Standard: 1. Dashboard offering insights with latest data available 2. 10% cost savings with better decionsion making ability 3. Saving business time 20% by eliminating manuall data cleaning process. 

There are few ways to collect data First, we can use the excel files or import the data from (OLTP - MySQL server) to OLAP (data wearhouse) and connect the wearhouse to POWER BI to create the dashboard. 

![alt text](https://github.com/arsadyum/Sales-Insight-with-Power-BI/blob/main/Power%20BI%20project%20image%201.JPG)

# Steps to complete the Power BI sales Data Insight project 

### Access Data: Accessing MySQL using Power BI get data icon ( server: localhost, database: sales) (user:root, password: ********)
### Load Selected data 
### Build a data model using star schema (Fact & Dimension table) 

![alt text](https://github.com/arsadyum/Sales-Insight-with-Power-BI/blob/main/Star%20Scema%20data%20model.JPG)

# Intial Data Transforming and Loading
## Remove Unnecessery Rows ( 0 & -1 sales amount) and Collumns
## Remove Duplicates 
## Add collumns using formula ( converting sales amount from INR to USD) 
## Rounding the values and create measures 
## Visualizing key insights on Power BI report 9 see below) 


![alt text](https://github.com/arsadyum/Sales-Insight-with-SQL-and-Power-BI/blob/main/Sales%20Insight%20Power%20BI%20Viz%20report.JPG)
