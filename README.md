# PROFIT ANALYSIS




### Project overview
This data analysis project aims to provide insights into the data from 50 startups in New York, California, and Florida. The features in this dataset are Administration Spending, Marketing Spending, R &D_ spend, location features, and Profit.By analysing these aspects of the startup's data ,we seek to identify trends, profits, make data-driven recommendation, and gain a deeper understanding of the startup's profits and performance.

### Data sources
The primary dataset used for this analysis is the "startups_data.csv" file, containing detailed information about each startup in New York, California, and Florida.

### Tools
- Excel - Data cleaning, Regression analysis
- SQL Server - Data analysis
- PowerBI - creating reports

### Data cleaning/preparation
In the initial data preparation phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

### Task
Perform Regression Analysis for the given data to identify how the money spent on Marketing, R&D, and Administration is affecting the company’s Profit. Predict the Profit for the below-given input features.

#### R&D Spend 
1. 21892.92
2. 23940.93         
#### Administration
1. 81910.77
2. 96489.63
#### Marketing Spends
1. 164270.7
2. 137001.1

### Regression Analysis
Regression analysis is a simple and statistical method to understand and quantify the relationship between two variables or more. It helps a business estimate one dependent variable based on the values of one or more independent variables.

The linear regression formula is represented as Y = mX +C , where
Y is the dependent variable.
X is the independent variable.
M is the estimated slope.
C is the estimated intercept.

In This project We have performed regression analysis to find out the profit and future profit prediction for the given value.


#### output:
![Screenshot 2024-02-16 184826](https://github.com/BhavaniAnchuri1/profit-analysis/assets/90407243/79fde445-88da-400f-8943-3c4ef1053de5)


### profit prediction
predicting the profit for the given input values

#### output:
![Screenshot 2024-05-02 215525](https://github.com/BhavaniAnchuri1/profit-analysis/assets/90407243/f62a41d7-7d40-414c-8a3f-624a267c611a)



### Data visualization
Power BI is a business intelligence tool that allows you to connect to various data sources, visualize the data in reports and dashboards, and then share them with anyone you want.
we have made dynamic and interactive dashboard for profit analysis using powerBI tool

![image](https://github.com/BhavaniAnchuri1/profit-analysis/assets/90407243/314cf07d-4924-4c59-8bc0-5db2f3c32f46)


### Data Analysis
I have performed some SQL queries to get desired output connected to server Data base extracted dataset and run the queries.

```sql
select*from startup;
select max(profit) as max profit from startup;
select sum(profit) as total profit from startup;
select sum(RD spend) as total RD spend from startup;
select sum(Administration) as total admi spend from startup;
select sum(Marketing Spend) as total mkt spend from startup;
select state, max(profit) as Total profit, max(RD spend) as Total RD spend, max(Administration) as Total admi spend, max(marketing spend) as total mkt spend from startup where state in ('New  York',’ California’,’  florida ')group by state  order by total profit desc;
select state, min(profit) as Total profit, min(RD spend) as Total RD spend, min(Administration) as Total admi spend, min(marketing spend) as total mkt spend from startup where state in ('New  York',’ California',’ florida ')group by state order by total profit desc;
```
### Results
- Regression analysis was performed to establish the relationship between various factors (R&D spending, administration spending, marketing spending) and profit. The regression model can predict profit based on these input variables.
- SQL queries were executed to retrieve various profit metrics like maximum profit, total profit, spending breakdown (R&D, administration, marketing) across different states.
- An interactive Power BI dashboard was created for data visualization, allowing dynamic analysis of profit and related factors.

### Observations
- The regression analysis showed that R&D spending, administration spending, and marketing spending all have an impact on the profit of startups.
- The SQL queries revealed that startups in New York had the highest total profit, while those in Florida had the lowest total profit among the three states analyzed.
- The SQL queries also provided insights into the total spending on R&D, administration, and marketing across different states.

### Recommendations
-  Utilize the regression model to forecast profit based on planned spending on R&D, administration, and marketing. This can aid in budget allocation and decision-making.
-  Focus on increasing R&D spending, as it likely has a positive impact on profit, based on the regression analysis.
-  Analyze the Power BI dashboard regularly to monitor profit trends, identify top-performing startups/states, and make data-driven decisions for improving profitability.
-  For startups in Florida, review their spending patterns and strategies, as they seem to be underperforming compared to startups in New York and California.
-  Continuously update the dataset and refine the analysis to incorporate any new factors or changes that may influence profitability.

### Conclusion
Overall, this project demonstrates the power of data analysis, regression modeling, and data visualization in understanding and optimizing profitability for startups. By implementing the recommendations, the company can make informed decisions to maximize profits and drive growth.










