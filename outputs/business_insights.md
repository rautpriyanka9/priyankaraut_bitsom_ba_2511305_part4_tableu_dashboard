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

# Business Insights

## Insight 1: Sales Trend Analysis

### Observation

Sales show an overall upward trend over the analysis period, with certain months experiencing significant spikes.

### Data Evidence

The Sales Trend dashboard indicates higher sales volumes during peak periods compared to surrounding months.

### Business Interpretation

Seasonal demand, promotions, or marketing campaigns may be driving these sales increases.

### Recommended Action

Investigate the factors contributing to peak-performing periods and replicate successful strategies in lower-performing months.

---

## Insight 2: Regional Performance

### Observation

One region consistently generates higher sales and profit than other regions.

### Data Evidence

The Regional Performance chart shows the highest sales and profit contribution from the top-performing region.

### Business Interpretation

The region may benefit from stronger market demand, better customer acquisition, or more effective sales operations.

### Recommended Action

Analyze best practices in the leading region and evaluate opportunities to replicate them in underperforming regions.

---

## Insight 3: Category Profitability

### Observation

Certain categories generate strong sales but relatively low profit margins.

### Data Evidence

The Category Profitability view shows a gap between sales volume and profitability for selected categories.

### Business Interpretation

High revenue does not necessarily translate into strong profitability due to discounts, costs, or operational inefficiencies.

### Recommended Action

Review pricing strategies and cost structures for low-margin categories.

---

## Insight 4: Sub-Category Performance

### Observation

Some sub-categories contribute disproportionately to profits while others generate losses.

### Data Evidence

The Category Profitability chart identifies profitable and loss-making sub-categories.

### Business Interpretation

Product mix optimization may improve overall business performance.

### Recommended Action

Increase investment in high-performing sub-categories and investigate causes of losses in underperforming products.

---

## Insight 5: Customer Segment Behavior

### Observation

One customer segment contributes significantly more sales and profit than other segments.

### Data Evidence

The Customer Segment dashboard view shows the largest revenue contribution from the leading segment.

### Business Interpretation

The business may be highly dependent on a specific customer group.

### Recommended Action

Develop targeted marketing and retention programs for the most valuable segment while exploring growth opportunities in smaller segments.

---

## Insight 6: Discount Impact on Profitability

### Observation

Higher discounts are generally associated with lower profit levels.

### Data Evidence

The Discount vs Profit scatter plot shows reduced profitability for transactions with larger discounts.

### Business Interpretation

Aggressive discounting may drive sales volume but erode margins.

### Recommended Action

Establish discount thresholds and evaluate whether discounts are generating sufficient incremental revenue.

### Follow-Up Question

What is the optimal discount level that maximizes both sales and profit?

---

## Insight 7: Shipping and Delivery Performance

### Observation

Certain shipping modes have longer average delivery times than others.

### Data Evidence

The Shipping Performance view shows differences in average delivery days across shipping methods.

### Business Interpretation

Long delivery times may negatively affect customer satisfaction and repeat purchases.

### Recommended Action

Review logistics performance and identify opportunities to improve delivery speed for slower shipping modes.

### Follow-Up Question

Do longer delivery times correlate with higher return rates or lower customer ratings?

---

## Insight 8: Return Pattern Analysis

### Observation

Specific categories, regions, or customer segments exhibit higher return rates.

### Data Evidence

The Return Analysis chart highlights groups with above-average return rates.

### Business Interpretation

Returns may indicate product quality issues, inaccurate customer expectations, or fulfillment problems.

### Recommended Action

Investigate high-return areas and implement corrective actions such as quality improvements, clearer product information, or enhanced customer support.

---

## Insight 9: Business Risk

### Observation

Profitability appears concentrated in a limited number of regions, products, or customer segments.

### Data Evidence

Dashboard analysis shows uneven contribution across business dimensions.

### Business Interpretation

Dependence on a small number of revenue drivers increases business risk.

### Recommended Action

Diversify revenue sources and expand successful strategies across additional markets and customer segments.

---

## Insight 10: Business Opportunity

### Observation

Several high-sales areas demonstrate strong profit margins and low return rates.

### Data Evidence

Combined analysis of sales, profitability, and returns identifies high-performing business segments.

### Business Interpretation

These segments represent opportunities for accelerated growth and investment.

### Recommended Action

Allocate additional marketing, inventory, and operational resources to scale these successful areas and maximize returns.
