# Analyzing customer churn in Power BI

Churn rate, also known as rate of attrition or customer churn, is the rate at which customers stop doing business with an entity. 

```
Churn rate = customers lost / total number of customers
```

- Churn rate calculation formula might differ from industry to industry. 

I followed the steps below to analyze and present an effective data visualization in this case study. 

1.	Data check
2.	Explore data and cleaning
3.	Analyze and visualization of the data
4.	Dashboarding
5.	Communicating insights

## Data check , Explore and cleaning
1. Check for "Column Quality" and "Column Distribution" features to profile data and identify potential issues such as missing values, outliers, or inconsistent data.
2. Handling Missing Values - Use the "Replace Values" or "Fill Down" options to replace missing values with appropriate values.
3. Use the "Remove Rows" option to remove rows with missing values if they cannot be filled.
4. Data Type Conversion - Ensure each column has the correct data type. Use the "Change Type" option to convert data types if necessary.
5. Removing Duplicates- Use the "Remove Duplicates" option to remove duplicate rows from your dataset.
6. Standardize data formats, such as date formats or text casing, to ensure consistency.

## Analyzing and visualization of data

1. understanding the data and formation of Data Modeling.
2. The creation of new DAX measures for required visualization.

Example : 
- AgeGroup new measure preparation

```
AgeGroup = 
SWITCH(
    TRUE(),
    'Databel - Data'[Age] < 30, "0-29",
    'Databel - Data'[Age] < 60, "30-59",
    "60+"
)
```
## Dashboard preparation and storytelling
Dashboard consists of 3 pages. 
- Overview
- Age groups, payments, and contracts analysis
- International data plans and insights

### Overview page 


![overview](https://github.com/anoshanimalirangalla/customer_churn_analysis/assets/164900866/7e011fe1-0cda-4f8e-99b8-194c1617dc65)


### Age groups, payments, and contracts analysis 


![age groups](https://github.com/anoshanimalirangalla/customer_churn_analysis/assets/164900866/4a31da04-9d3b-4119-aaa3-43c7d259a5f8)


### International data plans and insights 


![international plans](https://github.com/anoshanimalirangalla/customer_churn_analysis/assets/164900866/9d62bf00-4941-410f-824a-cf7ec0361d25)
