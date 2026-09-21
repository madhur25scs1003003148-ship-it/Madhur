# Data Quality Summary – Customer Churn

## Dataset overview
- Records: 15
- Columns: 11
- Duplicate rows: 0
- Duplicate Customer IDs: 0
- Missing values: 0

## Data types
- CustomerID: object
- Gender: object
- Age: int64
- TenureMonths: int64
- SubscriptionType: object
- MonthlyCharges: float64
- TotalCharges: float64
- ContractType: object
- SupportTickets: int64
- PaymentMethod: object
- Churn: object

## Outlier check (IQR method)
No IQR-based outliers were detected in the numeric columns.
- Age: 0 outliers (bounds 4.50 to 72.50)
- TenureMonths: 0 outliers (bounds -23.00 to 57.00)
- MonthlyCharges: 0 outliers (bounds -47.51 to 212.49)
- TotalCharges: 0 outliers (bounds -3689.82 to 7349.46)
- SupportTickets: 0 outliers (bounds -3.50 to 8.50)

## Summary statistics

| Metric | Age | TenureMonths | MonthlyCharges | TotalCharges | SupportTickets |
|---|---|---|---|---|---|
| count | 15.00 | 15.00 | 15.00 | 15.00 | 15.00 |
| mean | 39.07 | 18.80 | 84.66 | 2088.48 | 2.53 |
| std | 11.39 | 14.33 | 42.74 | 2407.37 | 1.92 |
| min | 23.00 | 2.00 | 49.99 | 99.98 | 0.00 |
| 25% | 30.00 | 7.00 | 49.99 | 449.91 | 1.00 |
| 50% | 38.00 | 15.00 | 79.99 | 1099.78 | 2.00 |
| 75% | 47.00 | 27.00 | 114.99 | 3209.73 | 4.00 |
| max | 60.00 | 48.00 | 149.99 | 7199.52 | 6.00 |

## Initial churn pattern
- Churn = Yes: 7 records
- Churn = No: 8 records

## Cleaning decisions
- Checked for missing values: none found, so no imputation was required.
- Checked for duplicate rows and Customer IDs: none found, so no records were removed.
- Checked numeric columns for IQR-based outliers: none found, so no values were capped or removed.
- Preserved the original valid categories and numeric values.