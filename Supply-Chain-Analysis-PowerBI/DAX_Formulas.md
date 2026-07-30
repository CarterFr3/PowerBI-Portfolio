# DAX Formulas Used

### 1. Average Lead Time (Days)
Average Lead time (days) = 
AVERAGE(Fact_Supplychain[Lead time]) & " Days"

Used In: AVG Lead Time KPI card
Why: Added the word "Days" for better readability on the card.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
### 2. Gross Profit
Gross Profit = 
SUM(Fact_Supplychain[Revenue generated]) - SUM(Fact_Supplychain[Costs])

Used In: Gross Profit KPI card + “Revenue & Gross Profit by Product Type” bar chart
Why: Needed a clear profit calculation to compare against revenue.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
### 3. Profit Margin %
Profit Margin % = 
DIVIDE(
    [Gross Profit],
    SUM(Fact_Supplychain[Revenue generated]),
    0
)

Used In: Profit Margin KPI card
Why: Used DIVIDE to safely handle cases where revenue might be zero.
