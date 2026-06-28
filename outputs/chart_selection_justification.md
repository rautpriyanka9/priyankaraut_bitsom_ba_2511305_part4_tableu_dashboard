# Chart Selection Justification

## Task 6: Visualization Design Principles

This dashboard was designed using established data visualization best practices to ensure that business stakeholders can quickly understand performance, identify trends, and make informed decisions.

---

## 1. Sales Trend View

### Business Question

How are sales changing over time?

### Chart Type

Line Chart

### Justification

A line chart is the most appropriate visualization for time-series analysis because it clearly displays trends, growth patterns, seasonality, and fluctuations over time. It allows executives to quickly identify periods of strong or weak sales performance.

### Design Principles Applied

* Chronological ordering of dates
* Clear axis labels
* Minimal clutter
* Consistent sales color throughout the dashboard

---

## 2. Regional Performance View

### Business Question

Which regions contribute the most sales and profit?

### Chart Type

Horizontal Bar Chart

### Justification

Bar charts provide straightforward comparison between regions. Horizontal bars improve readability when category names are longer and allow easy ranking of regional performance.

### Design Principles Applied

* Sorted from highest to lowest sales
* Profit displayed using color encoding
* Consistent formatting across regions
* Clear labels for comparison

---

## 3. Category Profitability View

### Business Question

Which categories and sub-categories drive profits or losses?

### Chart Type

Bar Chart

### Justification

Bar charts effectively compare profit values across categories and sub-categories. Positive and negative values are easy to distinguish, making it simple to identify profitable and loss-making product groups.

### Design Principles Applied

* Profit-based color coding
* Sorted values for easier interpretation
* Clear category hierarchy
* Focus on business outcomes

---

## 4. Customer Segment View

### Business Question

Which customer segments generate the strongest performance?

### Chart Type

Bar Chart

### Justification

Customer segments represent discrete categories that are best compared using bar charts. This visualization enables quick comparison of sales and profitability across segments.

### Design Principles Applied

* Consistent scales
* Direct comparison between segments
* Simple labeling
* Minimal visual distractions

---

## 5. Shipping Performance View

### Business Question

Which shipping modes experience longer delivery times?

### Chart Type

Bar Chart

### Justification

Shipping modes are categorical variables, making a bar chart the most effective option for comparing average delivery times and identifying operational bottlenecks.

### Design Principles Applied

* Delivery delays categorized using Shipping Delay Buckets
* Easy comparison of shipping methods
* Meaningful color usage
* Clear labels and sorting

---

## 6. Discount vs Profit View

### Business Question

What is the relationship between discounts and profitability?

### Chart Type

Scatter Plot

### Justification

A scatter plot is the most appropriate chart for analyzing relationships between two continuous variables. It helps identify trends, correlations, and outliers that may affect profitability.

### Design Principles Applied

* Each mark represents an observation
* Categories differentiated by color
* No misleading aggregation
* Clear interpretation of discount impact

---

## 7. Return Analysis View

### Business Question

Which categories, regions, or customer segments have the highest return rates?

### Chart Type

Bar Chart

### Justification

Return rates are best compared using bar charts because differences between categories can be easily identified and ranked.

### Design Principles Applied

* Sorted from highest to lowest return rate
* Clear percentage formatting
* Focus on risk identification
* Easy stakeholder interpretation

---

# Dashboard Design Principles Applied

## Correct Chart Selection

Each visualization was chosen based on the business question being answered. Line charts were used for trends, bar charts for comparisons, and scatter plots for relationships.

## Clear Visual Hierarchy

The dashboard places KPI cards at the top, followed by trend analysis and detailed performance views, guiding users from summary metrics to deeper insights.

## Minimal Clutter

Unnecessary gridlines, excessive colors, and decorative elements were removed to improve readability.

## Consistent Color Usage

A consistent color scheme was applied:

* Sales: Blue
* Profit: Green
* Losses: Red
* Returns: Orange

This improves recognition and reduces cognitive load.

## Proper Labels

All charts include descriptive titles, axis labels, legends where required, and formatted values.

## Readable Titles

Worksheet titles clearly describe the business question being answered.

## Appropriate Sorting

Bar charts are sorted by performance metrics to help users identify top and bottom performers quickly.

## Useful Filters

Interactive filters were added for:

* Region
* Category
* Customer Segment
* Order Date
* Ship Mode

These filters allow users to explore specific business scenarios.

## Avoidance of Misleading Scales

Axes use consistent scales and appropriate aggregation methods. No truncated axes or distorted visualizations were used.

## Focus on Business Interpretation

The dashboard emphasizes actionable business insights, including profitability, regional performance, customer behavior, shipping efficiency, and return risk, enabling data-driven decision making.

# Chart Selection Justification

## 1. Sales Trend View

### Question Answered

How are sales changing over time?

### Chart Type

Line Chart

### Why This Chart Is Appropriate

A line chart is the best choice for time-series analysis because it clearly shows trends, growth patterns, seasonality, and fluctuations across dates.

### Fields Used

* X-Axis: Order Date
* Y-Axis: Sales
* Filter: Region, Category, Customer Segment, Date

### Design Principle Applied

Chronological ordering and clear trend visualization.

### Mistake Avoided

Avoided using a bar chart for long-term trend analysis, which would make patterns harder to identify.

---

## 2. Regional Performance View

### Question Answered

Which regions generate the highest sales and profit?

### Chart Type

Horizontal Bar Chart

### Why This Chart Is Appropriate

Bar charts enable quick comparison across discrete categories and make ranking easy to understand.

### Fields Used

* Category Field: Region
* Measure: Sales
* Color: Profit
* Filters: Date, Customer Segment, Category

### Design Principle Applied

Sorted bars from highest to lowest performance to improve readability.

### Mistake Avoided

Avoided pie charts, which make regional comparisons difficult when multiple categories exist.

---

## 3. Category Profitability View

### Question Answered

Which categories and sub-categories drive profitability?

### Chart Type

Bar Chart

### Why This Chart Is Appropriate

Bar charts clearly compare profit values and highlight differences between categories and sub-categories.

### Fields Used

* Category: Category, Sub-Category
* Measure: Profit
* Color: Profit
* Filter: Region, Customer Segment

### Design Principle Applied

Used color to distinguish profitable versus loss-making categories.

### Mistake Avoided

Avoided stacked charts that could obscure profitability comparisons.

---

## 4. Customer Segment Analysis

### Question Answered

Which customer segments contribute the most revenue?

### Chart Type

Bar Chart

### Why This Chart Is Appropriate

Customer segments are discrete groups that are best compared using side-by-side bars.

### Fields Used

* Category: Customer Segment
* Measure: Sales
* Label: Sales Value
* Filters: Region, Date

### Design Principle Applied

Direct comparison of segment performance using consistent scales.

### Mistake Avoided

Avoided using multiple pie charts that would reduce comparison accuracy.

---

## 5. Shipping Performance View

### Question Answered

Which shipping modes have the longest delivery times?

### Chart Type

Bar Chart

### Why This Chart Is Appropriate

Bar charts effectively compare average delivery performance across shipping methods.

### Fields Used

* Category: Ship Mode
* Measure: Average Delivery Days
* Color: Shipping Delay Bucket
* Filters: Region, Category

### Design Principle Applied

Color coding was used to highlight delivery performance categories.

### Mistake Avoided

Avoided line charts because shipping modes are categorical rather than sequential.

---

## 6. Discount vs Profit View

### Question Answered

How do discounts affect profitability?

### Chart Type

Scatter Plot

### Why This Chart Is Appropriate

Scatter plots are ideal for identifying relationships between two continuous variables and spotting outliers.

### Fields Used

* X-Axis: Discount
* Y-Axis: Profit
* Color: Category
* Size: Sales
* Filters: Region, Customer Segment

### Design Principle Applied

Visualized correlation while preserving individual transaction-level variation.

### Mistake Avoided

Avoided aggregating data into bars, which would hide the relationship between discount and profit.

---

## 7. Return Analysis View

### Question Answered

Which categories, regions, or customer segments have the highest return rates?

### Chart Type

Bar Chart

### Why This Chart Is Appropriate

Bar charts allow easy comparison of return rates across groups and help identify areas of operational concern.

### Fields Used

* Category: Category or Region
* Measure: Return Rate
* Color: Return Rate
* Filters: Customer Segment, Date

### Design Principle Applied

Sorted categories by return rate to emphasize the highest-risk areas.

### Mistake Avoided

Avoided unsorted tables that would make return patterns difficult to identify.

---

# Dashboard-Level Design Principles

## Clear Hierarchy

The dashboard begins with KPI cards, followed by trend analysis and then detailed performance breakdowns. This guides leadership from summary metrics to root-cause analysis.

## Consistent Color Usage

* Sales: Blue
* Profit: Green
* Losses: Red
* Returns: Orange

Consistent colors improve interpretation and reduce confusion.

## Minimal Clutter

Unnecessary gridlines, decorative visuals, and redundant legends were removed to keep focus on business insights.

## Readable Titles and Labels

Every chart uses descriptive titles and clearly labeled axes to ensure non-technical stakeholders can understand the findings.

## Appropriate Sorting

Bar charts are sorted by performance measures to make top and bottom performers immediately visible.

## Useful Filters

Interactive filters allow users to analyze performance by:

* Region
* Category
* Customer Segment
* Date
* Ship Mode

## Avoidance of Misleading Scales

Axes begin at appropriate baselines, and visualizations avoid distorted scales that could exaggerate differences.

## Focus on Business Interpretation

All visualizations were selected to support business decision-making related to sales growth, profitability, operational efficiency, customer behavior, and risk management.
