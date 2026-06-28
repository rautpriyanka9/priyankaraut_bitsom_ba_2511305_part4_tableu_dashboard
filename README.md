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