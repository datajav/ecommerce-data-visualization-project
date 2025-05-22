# Ecommerce-data-visualization-project

E-commerce Customer Analytics Dashboard
Project Overview
This repository contains a comprehensive data analytics project which analyzes customer behavior and sales performance using Power BI for visualization and Python for data preprocessing. It utilizes a synthetic e-commerce dataset with customer demographics, transaction details, product information, and customer reviews to generate actionable business insights.

Customer demographics (ID, gender, age)
Product information (ID, name, category)
Transaction details (order date, quantity, price)
Customer experience metrics (payment method, review score)
Geographic information (city)

Analysis Scope

This dashboard provides multi-dimensional insights into:

Sales Overview (Revenue trends & order volume)
Customer Demographics (Age & gender segmentation)
Geographic Analysis (Sales distribution by city/region)
Product Performance (Top-selling categories & products)
Customer Satisfaction & Loyalty (Review scores & retention metrics)

Executive Summary 

With creating this dashboard here are the findings identifed for each metric. The highest quantity of items were sold in December 2024.

![image](https://github.com/user-attachments/assets/3f7957dc-d9f4-49d6-af23-e2f813be394d)

*Electronics* contributed the most to overall sales. 

![image](https://github.com/user-attachments/assets/b61db39e-67f6-42d8-83bf-a88d5577d850)

Customers typically spent $87.76 per order, indicating a stable purchase behavior. The highest spending age bracket was 60-70, showing stronger purchasing power. Female customers made %44.56 more purchases, influencing targeted promotions. We can See as well the the Top Performing Cities: East Robert, South Tonya, Port Melissaborough generated the most revenue.

Average Review Score: Customers rated products 3.99/5 on average, indicating reletively positive feedback.

![image](https://github.com/user-attachments/assets/18baa571-5546-4995-a887-72ef7a483cc7)


Technical Implementation

Data Cleaning: Removing duplicates, handling missing values with Data Wrangler.
Feature Engineering: Creating calculated fields like Age Groups or Customer Segments.
Statistical Analysis: Using Pandas & NumPy for deeper insights.
Export to Power BI: Processed data is saved as a .csv for Power BI import

Key Visualizations:

Time-series analysis of sales performance
Geographic distribution maps
Product category treemaps
Customer demographic breakdowns
Review score distribution analysis
Payment method comparison
Business Applications

Highlight real-world use cases:

✔ Targeted Marketing Strategies
✔ Customer Retention Optimization
✔ Product Demand Forecasting
✔ Geographic Expansion Insights
Future Enhancements

Recommendations
Based on the analysis, propose actionable recommendations:

1. Improve Customer Retention Strategies
Offer personalized promotions based on purchasing behavior.
Implement a loyalty program targeting high-value returning customers.
Address low review scores by identifying common customer pain points.

2. Optimize Marketing Efforts
Focus marketing campaigns on top-performing age segments.
Enhance regional targeting by investing in locations with high sales growth.

3. Streamline Product Offerings
Prioritize stocking best-selling products and discontinue underperforming items.
Enhance pricing strategies based on demand analysis and customer spending habits.

Microsoft Power BI Desktop
DAX (Data Analysis Expressions)
Power Query M Language
Data visualization best practices
Python Data Wrangler
