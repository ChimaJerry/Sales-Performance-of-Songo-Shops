# Sales-Analysis-SQL
This is an ETL project on the data set of Songo chains of retail shop to gather insight into her business activities to enhance decision making

### Table of Content
- [Project Overview](#project-overview)
- [Skills Used](#skills-used)
- [Data Source](#data-source)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)
- [Recommendation](#recommendation)

### Project Overview
 The dataset is a synthetic data of purchases in a retail shop that reflects happenings in a real-world scenario. The data has been carefully crafted to reflect the  demography of customers and purchase pattern in a retail shop.  It is a sample of 1000 transactions that customers have made with a retail shop between January 2023 – January 2024.

### Skills Used

- Excel - Data Cleaning
- SQL Server - Data Analysis
- Power BI - Data Visulaization
- RStudio - Some Data visualization unattainable with Power BI.
  
### Data Source
The selected data set was gotten online from Kaggle [here](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset/discussion?select=retail_sales_dataset.csv)


### Data Cleaning and Preparation

 In the initial phase of the data cleaning the following tasks were performed;
- Data Loading and inspections
- Duplicate or missing values was checked
- Data cleaning and formatting

### Exploratory Data Analysis
Exploratory data analysis was conducted to understand the data structure, data types,  and descriptive summary statistics conducted to better understand the dataset.  For this data set the transaction ID and Customer ID was identified as the possible unique feature or primary key of the data set. Went ahead to using advance data analysis feature of excel to get an insight into some summary of the numerical data in the data set. This analysois intends to knpow the following from the dataset.
1. Month with the highest sales.
2. Product category sold the most and least.
3. Total quantity sold in each month.
4. Total revenue generated from sales.
5. Average age of most shoppers.
6. Which gender purchase a given product the most.
7. Which product was purchased the most by specific male and female gender.

### DATA Analysis
SQL server was used to interact witht the dataset. Here are some example of SQL queries you can run against the database:
#### sales revenue for each month:
``` sql
SELECT DATE_TRUNC('month', sale_date) AS month, SUM(quantity * price) AS total_sales
FROM sales
GROUP BY month
ORDER BY month;
```


### Results and Findings

### Recommendations

### Limitations

