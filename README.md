# Project: Telco Churn Customer Analysis
The dataset contains customer information from a telecommunications / subscription-based service company, that requires investigation of churn dynamics over a wide range of consumer profiles and behaviors. This study will help guide strategic decisions targeted at increasing customer satisfaction, retention, loyalty, and long-term profitability.

----------

# Project Objective:
To analyze the rate of customer churn across multiple categories. The project's goal is to identify insights into factors influencing customer retention and attrition by evaluating turnover rates across different categories. To provide actionable insights and recommendations for reducing churn, improving client retention methods, and optimizing company results.

--------

# Data Cleaning:
The data was cleaned and manipulated using Power Query in Microsoft Excel. For column - Senior Citizen, the data type was changed to text and the values 0 and 1 replaced by No and Yes, respectively. There were  < 1% empty cells in column – TotalCharges. I filtered the cell and studied the null values alongside side other cells in the column, and I noticed the customers were recently onboarded and yet to make any payments, so I replaced the null with 0, This will help to maintain data consistency, integrity, and compatibility, which are essential for accurate analysis and decision-making.
After the dataset was cleaned, I checked for duplicates and found none. Close and loaded to Microsoft Excel for analysis.

----------

# Data Transformation: 
Three (3) new columns were created to be used as metrics for the analysis.
Churn Count – This will be used to calculate the number of churn customer and find the rate. The IF formular [=IF([@Churn]="No",0,1)] was used to derive this from the dataset.
Customer Count – This will be used to calculate, Total number of customers. The COUNTIF formular [=COUNTIF([customerID],[@customerID])] was used to derive this from the dataset.
Two (2) new calculated field were created via the PivotTable analyze tab. 
ChurnRate - it was calculated using “Churn Count / Customer Count”.
NonChurn Customers – This was calculated using “Customer count – Churn Count”.

-----------

# Data Visualization: 
Data Visualization was done with Microsoft Excel depicting churn rate by Contracts, Partners, Senior Citizens and Dependant. It also shows the average monthly charge for each parameter.

---------

# Findings:
### The KPIs
Total Customers - 7043.
Churn Rate - 26.5%.
Churn Customers - 1869.
Not Churn Customers - 5174.
Average Monthly Charges - $64.76.

Month-to-month contracts have the highest churn rate at 42.7%, followed by one-year contracts at 11.3% and two-year contracts with the lowest at 2.8%. Churn rates range significantly depending on contract duration, with longer contracts resulting in lower churn rates. 
Customers on month-to-month contracts pay the highest average monthly fee of $66.40, followed by one-year contracts at $65.05, and two-year contracts with the lowest average monthly price of $60.77. Despite the disparity in churn rates, the average monthly prices vary very little between contract types.

Customers with partners have a reduced turnover rate of 19.7%, whereas those without partners have a higher churn rate (33.0%). This shows that having a partner is associated with a lower chance of turnover. 
Customers with partners pay an average monthly charge of $67.78, compared to $61.95 for those without partners. Despite their differences, both groups contribute to the aggregate average monthly charge of 64.76.

Senior citizens churn at a higher rate (41.7%) than non-senior citizens (23.6%). This suggests a considerable difference in turnover behaviour between seniors and non-senior persons. 
Senior citizens who churned paid a higher average monthly price of $79.82 than non-senior citizens who churned, which was $61.85. This shows that both groups follow similar trends, with consumers with higher monthly prices being more likely to churn.

Customers without dependents have a greater churn rate (31.3%) than those with dependents (15.5%). Customers who have dependents have lower churn rates.
 Customers without dependents have higher average monthly expenses of $67.00, but those with dependents have lower average monthly charges of $59.52. Regardless of attrition rates, there is a difference in average monthly prices for customers with and without dependents.

--------

# Recommendations: 
Contracts category: encouraging customers to opt for longer-term contracts through discounts and added benefits can stabilize churn rates. Improving the value proposition for month-to-month subscribers and strategically upselling them to one-year contracts can further bolster retention efforts. Ensuring satisfaction across all contract types is crucial for maintaining long-term customer relationships.
Partners category: it's vital to incentivize partnerships by offering promotions and discounts while ensuring solo customers feel their subscriptions are equally valuable. Tailoring marketing strategies to cater to the distinct needs of each group can enhance engagement. Additionally, implementing retention programs specifically designed for customers without partners can help mitigate churn rates. 
Senior Citizens Category: providing specialized offers and services tailored to this demographic can foster loyalty and retention. Enhancing the perceived value of subscriptions for senior citizens, along with offering personalized support and assistance, can help address their unique needs. Tailoring marketing messages to resonate with seniors and senior citizens can further enhance engagement and retention efforts.
Dependents category:  providing targeted discounts and services for customers with dependents can foster loyalty, while enhancing the value proposition for those without dependents can justify their subscription costs. Offering educational resources and support for customers with dependents can help them maximize the benefits of their subscriptions. Tailoring marketing strategies to address the unique needs of each group within this category can further strengthen retention efforts. 

---------

#### Thank you
