# Chicago Food Inspections Data Engineering Project

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
![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/28b42fd0-16e6-4741-bdeb-d3e19d16fdb6)

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/f3453bef-8d1a-4772-8a31-2bfbec5623f7)

## 2. Dynamic Dimensional Modeling:

Create a dynamic dimensional model using ER/Studio to facilitate efficient data analysis, enabling exploration of food inspection data across various dimensions and hierarchies.

![image](https://github.com/simran2097/Chicago_Food_Inspection/assets/47267975/ba8d84dc-8466-4499-86fe-b7d1b511effb)

## 3.Data Integration / ETL Pipeline:

The data integration and ETL pipeline is a two-layer process:

Landing or Staging Data Layer: Data is extracted from the source and staged into the SQL Server database with minimal transformation (as-is data load). Audit fields are added to identify newly loaded or updated records.

Schema: CHICAGO_INS

Table: STG_CHICAGO_FOOD_ESTD_INS

Dimensional Data Layer: Data is loaded into the multi-fact dimensional data warehouse after extraction and transformation with defined rules. Data quality checks are performed post data load, and audit columns are added to each dimension and fact for record audit and maintenance.

Schemas: CHICAGO_INS
Tables:
Dim_Chicago_BusinessLicenses
Dim_Chicago_FacilityType
Dim_Chicago_FoodInspectionResults
Dim_Chicago_FoodInspectionType
Dim_Chicago_FoodRiskCategory
Dim_Chicago_Geo
Dim_Chicago_Restaurants
Dim_Chicago_ViolationCodes_SCD
FCT_Chicago_FoodInspections_Violations
FCT_Chicago_FoodInspections
FCT_NYC_FoodInspection_Violations
