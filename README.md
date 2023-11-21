# Chicago Food Inspections Data Engineering Project
Desigining Advanced Data Architectures for Business Intelligence.

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/1d296a46-37b5-473a-8c62-55cd20dea7d0)

## Overview :

This repository contains the data engineering solution for analyzing restaurant inspections and violations happening in Chicago. The project involves data extraction, data cleansing, transformation, exploratory analysis, data visualization, and data flow orchestration of event data on the cloud. The goal of this project is to enable data-driven decisions, improve customer engagement, and drive business growth by providing insights into food establishment inspections in Chicago.

## Data Source:

The data for this project is sourced from the Chicago Data Portal. It includes information on inspections of restaurants and other food establishments in Chicago from January 1, 2010, to the present. Inspections are performed by staff from the Chicago Department of Public Health’s Food Protection Program using a standardized procedure. The dataset is updated daily and is available in CSV format.

## Data Description:

Number of Rows: 443,000

Number of Columns: 17

Update Frequency: Daily

File Format: CSV

## Tools Used:

ER/Studio Data Architect for data modeling.

Alteryx for data integration and ETL processes.

Microsoft SQL Server for data warehousing.

Power BI and Tableau for business intelligence reporting and visualization.

This dataset consists of below metadata information:

## 1. Data Profiling:
The project utilizes ER/Studio Data Architect to design and manage data models and metadata for the database. It involves creating conceptual, logical, and physical data models, mapping relationships and dependencies between them, and implementing a multi-fact dimensional model using normalization and schema design strategies.

### Alteryx Profiling Business License:

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/28b42fd0-16e6-4741-bdeb-d3e19d16fdb6)

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/f3453bef-8d1a-4772-8a31-2bfbec5623f7)

### Alteryx Profiling for Food Inspection:
![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/bafdb4ec-24d5-40a5-a8a1-52ce88027be5)

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/296f6991-2e6a-4b91-9a62-b5f073386c47)


## 2. Dynamic Dimensional Modeling:

Create a dynamic dimensional model using ER/Studio to facilitate efficient data analysis, enabling exploration of food inspection data across various dimensions and hierarchies.

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/ba8d84dc-8466-4499-86fe-b7d1b511effb)

## 3.Data Integration / ETL Pipeline:

The data integration and ETL pipeline is a two-layer process:

Landing or Staging Data Layer: Data is extracted from the source and staged into the SQL Server database with minimal transformation (as-is data load). Audit fields are added to identify newly loaded or updated records.

Schema: CHICAGO_INS

Table: STG_CHICAGO_FOOD_ESTD_INS

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/bdfab847-08f5-4158-9633-f7284265e8e6)


Dimensional Data Layer: 

Data is loaded into the multi-fact dimensional data warehouse after extraction and transformation with defined rules. Data quality checks are performed post data load, and audit columns are added to each dimension and fact for record audit and maintenance.

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/1653ac92-ff2e-4a73-b1e8-1f09995bd5d9)

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/0d12e53a-c1da-49ba-9469-f280316b3cb5)


## BI Reporting:

Business Intelligence reporting involves preparing, analyzing, and portraying business metrics to support decision making. This project leverages the potential of Power BI and Tableau to derive key business insights by identifying key measurements such as satisfaction level and applying dimensions such as inspection date, restaurant, and violation code information.

BI reports and dashboards have been developed to identify violations in health norms and regulations at restaurants and cafeterias in Chicago.

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/61cdd7a1-3233-4a73-a679-6084cacc0ba4)


![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/020011ca-5a62-4acc-9af9-1eb07edf1f74)


![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/8c6b3cad-32c6-42c5-b281-09ced05b11b9)
