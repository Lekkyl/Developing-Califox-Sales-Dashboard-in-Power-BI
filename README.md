# Developing-Califox-Sales-Dashboard-in-Power-BI
In this repo, I assumed the role of a BI Developer; creating a power BI sales report dashboard for Califox Ltd and published on power BI service for their Business Leaders to have access to fine grained reports tailed to requirements. 

## Situation
Califox is a newly established financial service provider offering payment as a service to it's customers. However, it's sales business leaders find it difficult to access their sales report because their data platform is somewhat difficult to use for non-data experts. Therefore, it has become a challenge for them to track business position on the fly, not to mention generating insights for business decision making.
As a newly recruited BI developer, it is my sole responsibility to bridge this gap by providing easily aceesible, easy-to-use and comprehensible report, and intelligence to all sales staff (both business leaders and their team members and management.

## Objectives
* Data and business Understanding
* Identify cost-effective data platform for hosting dashboard.
* Develop dashboard that would provide intelligence to all stakeholders from data system.

## Steps/Approach
After understanding the entities and their attributes and their business definitions and applications, I proceeded with the following steps;

### Data Preparation
* I downloaded excel files of fact datasets. There were two (2) fact datasets and each dataset was about a hundred and fifty thousand rows daily.
* Clean excel file to suit business requirements. I wrote four (4) macros that did this.
* Append cleaned data to history data (i.e already cleaned and stored data).

### Data Modelling
* Loaded data folder using power query, edited data types using query editor and created a reference table from one of the fact tables to serve as dimension table linking the two (2) fact tables.
* I created a star schema data model of five (5) dimension tables and two (2) fact tables to relate my datasets. Each of the fact tables has two (2) date columns, but one (1) in common.
![image](https://github.com/Lekkyl/Developing-Califox-Sales-Dashboard-in-Power-BI/assets/66248503/219c03a7-814c-4cc3-854f-bd029d2a5d94)

### Data Analysis
* I wrote quite a numnber of measures to analyze the data and make the dashboard robust for time intelligence. Some of which includes; 
    * Calculate
    * Basic arithmetic functions - sum, divide, minus (-), multiplication (*)
    * Time intelligence functions - dateadd, datesinperiod, eomonth, datediff, datesmtd, year, month, day, quarter, datesqtd, datetable, datesbetween
    * Conditionals - if, and, or, isweekday
    * Count, distinctcount
In total I wrote about 120 measures distributed over 7 measure tables and 8 calculated columns.

### Data Visualization
The main page of the dashboard was designed to give sales staff a simple and concise grasp of the major business metrics, KPI and trend analysis. Other pages show report of their customers' performance and activity.
![image](https://github.com/Lekkyl/Developing-Califox-Sales-Dashboard-in-Power-BI/assets/66248503/717d883a-77dc-4f98-a9b5-1ec1f042074a)
![image](https://github.com/Lekkyl/Developing-Califox-Sales-Dashboard-in-Power-BI/assets/66248503/ddeaa457-b0a4-45d9-8cea-a76ea90214b9)


### Publishing to Power BI
I created an onmicrosoft domain on Azure to share this project

Please feel free to explore this dashboard on the link below
[Link to dashboard](https://app.powerbi.com/view?r=eyJrIjoiOGM0MjVmODctNGNkZS00NjAyLTg5N2ItM2Q1NWJkNzEzMWRmIiwidCI6IjQzYjc2NzQxLTgzYWYtNGQ5Ny1hMDNhLThlNmNmMmFhMmVhMCIsImMiOjZ9&embedImagePlaceholder=true&pageName=ReportSectionb975dafc1fb4b66613b1)
