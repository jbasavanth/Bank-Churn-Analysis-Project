
### Bank Customer Churn Analysis – Detailed Project Overview
This project focuses on analyzing customer churn for a bank using Power BI. 
The primary objective was to understand the patterns of customer churn based on various demographic and financial metrics. 
By leveraging these insights, the bank could develop strategies to improve customer retention, reduce churn risk, and enhance overall decision-making.

Problem Statement
Customer churn is a significant challenge for banks and financial institutions, 
leading to lost revenue and a reduced customer base. 

The project aimed to address the following concerns:
Identifying patterns and trends in customer churn to determine which customer segments are most likely to leave the bank.
Understanding customer demographics (age, gender, credit score, tenure, account balance) and segmenting high-risk customers.
Developing Key Performance Indicators (KPIs) to measure customer retention and loss.
Providing actionable insights through interactive visualizations to help the bank make informed decisions and create effective retention strategies.


Project Structure
1. Data Cleaning and Preprocessing
The first phase focused on preparing the data for analysis:
- Use First Row as Header: Ensured that the first row of the dataset was set as the header.
![image](https://github.com/user-attachments/assets/21d70a4e-33d8-4652-8a71-e831381c877d)
- Remove Useless Columns: Irrelevant columns like estimated_salary were removed to avoid noise in the analysis.
![image](https://github.com/user-attachments/assets/e9eeaf80-3719-4341-97ef-369769397466)
- Rename Columns: Columns were renamed for clarity, making it easier to interpret the data in the final reports.
- Prepare Data Types: Validated and corrected each column’s data type (e.g., numbers, text, dates).
- Add Conditional Columns:
Created age groups (e.g., 20-30, 30-40) for easier customer segmentation.
![image](https://github.com/user-attachments/assets/4ef6379d-e3f6-45e5-aba7-d5f835928af9)

- Created credit Group (e.g., <=400, 401-500, 501-600, 601-700, 701-800, >800).
![image](https://github.com/user-attachments/assets/75959722-1bd7-4a17-8893-64aea767bf26)

- Defined account balance categories to segment customers based on their financial standing.
![image](https://github.com/user-attachments/assets/3999efdd-b384-4a5a-8c67-021b14e1a672)

- Replace Values: Simplified categorical values like credit card ownership (e.g., Owned (1) or Not Owned (0)) for better interpretation in the visualizations.
![image](https://github.com/user-attachments/assets/6ec48a39-10b2-40d2-a23a-038dacc236a3)


3. Data Modeling
The data was modeled and structured to optimize for querying and visualization in Power BI. Relationships between different variables, such as demographics and churn rates, were established to enable meaningful analysis.
![image](https://github.com/user-attachments/assets/c7de9036-a220-422d-a7fb-67ef76ead67b)


5. Key Performance Indicators (KPIs)
Using DAX (Data Analysis Expressions), several key metrics were calculated:
Total Number of Customers: The total customer count in the dataset.
![image](https://github.com/user-attachments/assets/abb954d4-d888-4a81-adbb-79b52c958d78)

Number of Customers Lost: The count of customers who churned during the analysis period.
![image](https://github.com/user-attachments/assets/de6ef988-d782-4b70-88cf-7e3f456e32da)

Churn Rate: The percentage of customers who left the bank, calculated using DAX measures.
![image](https://github.com/user-attachments/assets/6bab089e-b112-4872-b6cb-a50376fd6fc0)

4. Data Visualization
Interactive visualizations were created to display churn patterns clearly and intuitively:
Bar Charts: Illustrated churn across demographics such as age group, gender, tenure, and credit score.
Donut Charts: Showed overall churn rate percentages.
Interactive Slicers: Allowed filtering by various factors (e.g., gender, age group, credit score) to dynamically explore churn patterns across customer segments.
Financial Metrics Visualization: Plots and charts depicted relationships between churn and financial metrics like account balance, tenure, and credit score.

6. Analysis and Insights
Key insights from the analysis include:
Churn by Age Group:
High churn in younger customers (20-30): Younger customers exhibited higher churn rates, possibly indicating a need for tailored retention strategies targeting their financial needs.
Stable churn among mid-aged groups (40-60): These customers showed lower churn due to longer tenure and higher likelihood of using multiple financial products.
Increased churn in older customers (above 60): Older customers, nearing or in retirement, also displayed signs of churn, perhaps due to changing financial priorities.

Churn by Credit Score:
Lower credit scores linked to higher churn: Customers with poor or average credit scores were more likely to churn, likely due to financial instability.
High credit score customers show loyalty: Customers with high credit scores showed significantly lower churn rates, likely due to trust and usage of premium financial products.
Churn by Account Balance:

Lower account balances linked to churn: Customers with lower balances were at higher risk of leaving the bank.
Higher balance customers are more stable: These customers tend to rely on long-term financial products, leading to lower churn.
Churn by Tenure:

New customers (under 3 years) were more likely to churn, suggesting the need for improved onboarding and engagement efforts.
Longer tenure leads to better retention, with customers staying longer showing significantly lower churn.

Churn by Gender:
Both genders showed similar churn rates, but slight variations suggest the possibility of gender-specific retention efforts, with different financial product preferences.

Key Achievements
Comprehensive Churn Analysis: The analysis provided a complete picture of customer churn based on various factors, helping the business understand the key risk areas for customer attrition.
KPI Development: Using DAX measures, important metrics like churn rate, total customers, and lost customers were defined and could be monitored regularly.
Interactive Slicers: Allowed users to filter and explore different combinations of demographic and financial data, giving a deeper understanding of churn patterns.
Data Cleaning & Preprocessing: Structured the data effectively to ensure accurate analysis and meaningful insights.
