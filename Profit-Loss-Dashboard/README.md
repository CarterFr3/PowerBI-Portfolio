# US Stores Profit & Loss Dashboard

## Project Overview
This Power BI project analyzes sales and profitability data from US retail stores. The goal is to evaluate revenue, cost of goods sold (COGS), gross profit, expenses, and how actual costs compare to budget.

## Business Questions Answered
- What is the overall profitability of the business?
- How do actual COGS compare to the budgeted COGS?
- Which product types and individual products generate the most profit?
- Which states and regions perform best in sales and profit?
- How does performance vary across different time periods?

## Key Insights
- **Columbian** and **Coffee** are the top products by profit.
- Actual COGS exceeded the budget in every quarter.
- **California** and the **West** region lead in both sales and profit.
- Overall profit margin is approximately **31.7%**.

## Skills Demonstrated
- Star Schema data modeling
- DAX measures
- Budget vs Actual analysis
- Interactive dashboard design
- Data storytelling

## DAX Measures Used
- **Gross Profit** = `SUM(Fact[Profit])`
- **Total COGS** = `SUM(Fact[COGS])`
- **Profit Margin %** = `DIVIDE([Gross Profit], SUM(Fact[Sales]), 0)`

## Dashboard Features
- KPI cards for Total Sales, Total COGS, Gross Profit, Profit Margin %, and Total Expenses
- Profit, COGS and Sales comparison by Product Type
- Actual COGS vs Budget gauge
- Profit by Product
- Sales and Profit by State
- Sales by Region (donut)
- Top 10 Products by Profit
- Slicers for Year, Quarter, Month, State, Product Type, and Market

## Tools Used
- Power BI Desktop
- DAX
- Power Query
