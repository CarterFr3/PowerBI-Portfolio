# DAX Formulas Used

### 1. Gross Profit
Gross Profit = SUM(Fact[Profit])

Used In: Gross Profit KPI card
Why: Uses the existing Profit column to show overall profitability.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
### 2. Total COGS
Total COGS = SUM(Fact[COGS])

Used In: Total COGS KPI card and Actual COGS vs Budget gauge
Why: Needed to track actual cost of goods sold and compare it against the budget.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
### 3. Profit Margin %
Profit Margin % = 
DIVIDE(
    [Gross Profit],
    SUM(Fact[Sales]),
    0
)

Used In: Profit Margin % KPI card
Why: Shows what percentage of sales is retained as profit. DIVIDE is used to safely handle any potential division by zero.
