# Task 1: Connect and Inspect Data

## Dataset Overview

The dataset was loaded into Tableau from `dashboard_sales_data.xlsx`.

- Total Records: 4,200
- Total Fields: 20

## Field Classification

### Date Fields
| Field Name | Data Type |
|------------|-----------|
| order_date | Date |
| ship_date | Date |

### Geographic Fields
| Field Name | Data Type |
|------------|-----------|
| region | String |
| state | String |
| city | String |

### Categorical Fields
| Field Name |
|------------|
| order_id |
| customer_id |
| customer_segment |
| category |
| sub_category |
| product_name |
| ship_mode |
| campaign_channel |

### Numerical Measures
| Field Name | Data Type |
|------------|-----------|
| sales | Decimal |
| quantity | Integer |
| discount | Decimal |
| profit | Decimal |
| delivery_days | Integer |
| customer_rating | Decimal |

### Binary / Flag Fields
| Field Name | Description |
|------------|-------------|
| return_flag | 0 = Not Returned, 1 = Returned |

## Data Type Validation

The data types detected in Tableau match the expected business meaning:

- Dates are correctly identified as Date fields.
- Geographic dimensions are stored as text/string fields.
- Sales and profit metrics are stored as numeric measures.
- Return status is represented as a binary flag.
- Customer ratings are stored as decimal values.

## Assumptions

1. Each row represents a unique order transaction.
2. `order_id` uniquely identifies an order.
3. `sales` represents total revenue generated from the order.
4. `profit` represents net profit earned from the order.
5. `return_flag` uses:
   - 0 = Order not returned
   - 1 = Order returned
6. `delivery_days` represents the number of days between order and delivery.
7. Geographic fields (`region`, `state`, `city`) are used for location-based analysis.
8. `customer_rating` is assumed to be measured on a 1–5 scale.
9. No changes were made to the source data during import.

## Initial Data Quality Observations

- Date fields were successfully recognized.
- No obvious data type mismatches were detected.
- Geographic hierarchy exists at Region → State → City level.
- Dataset contains both transactional and customer experience metrics, enabling sales, profitability, delivery, and customer satisfaction analysis.

## Task 3: Tableau Views Created

The following worksheets were created:

1. Sales Trend View
   - Line chart showing sales over time.

2. Regional Performance View
   - Bar chart comparing sales and profit across regions.

3. Category Profitability View
   - Category and sub-category level profit analysis.

4. Customer Segment View
   - Performance comparison across customer segments.

5. Shipping Performance View
   - Delivery performance by shipping mode and delay bucket.

6. Discount vs Profit View
   - Scatter plot analyzing the relationship between discounts and profitability.

7. Return Analysis View
   - Return rate analysis by category, region, and customer segment.

These views were combined into an interactive Tableau dashboard with global filters for Region, Category, Customer Segment, and Date.

## Task 4: Appropriate Chart Selection

The dashboard uses chart types that align with the underlying business questions:

| Business Question | Chart Type | Reason |
|------------------|------------|---------|
| Sales trend over time | Line Chart | Best for trend analysis |
| Regional performance | Bar Chart | Easy comparison between regions |
| Category profitability | Bar Chart | Clear profit comparison across categories |
| Customer segment performance | Bar Chart | Effective segment comparison |
| Shipping delays by mode | Bar Chart | Highlights delivery performance differences |
| Discount vs Profit | Scatter Plot | Shows relationship between two numerical measures |
| Return Analysis | Bar Chart | Compares return rates across groups |

All chart selections prioritize clarity, comparability, and business decision-making while avoiding misleading or decorative visualizations.
