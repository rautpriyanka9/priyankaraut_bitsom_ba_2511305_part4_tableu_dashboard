## Task 2: Calculated Fields

Five calculated fields were created in Tableau:

### 1. Profit Margin
Formula:
SUM([Profit]) / SUM([Sales])

Purpose:
Measures profitability as a percentage of sales.

### 2. Cost
Formula:
[Sales] - [Profit]

Purpose:
Estimates cost associated with generating sales.

### 3. Average Order Value
Formula:
SUM([Sales]) / COUNTD([Order ID])

Purpose:
Measures average revenue generated per order.

### 4. Return Rate
Formula:
SUM([Return Flag]) / COUNT([Order ID])

Purpose:
Measures the percentage of orders returned.

### 5. Shipping Delay Bucket
Formula:
IF [Delivery Days] <= 3 THEN "Fast Delivery"
ELSEIF [Delivery Days] <= 7 THEN "Normal Delivery"
ELSE "Delayed Delivery"
END

Purpose:
Categorizes delivery performance into actionable groups.