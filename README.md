# E-commerce Data Quality and Automation

## Project Overview
This project analyzes an e-commerce product dataset from Kaggle to identify data quality issues, clean product information, validate prices and discounts, and generate useful business insights using Python.

## Tools and Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab
- Kaggle dataset

## Project Workflow
1. Downloaded and explored the dataset.
2. Profiled missing values and duplicate records.
3. Standardized column names.
4. Converted prices, discounts, and recent-sales indicators into numeric columns.
5. Removed exact duplicate rows.
6. Handled missing product names using an alternative title column.
7. Validated prices and discount ranges.
8. Flagged products priced above $500 for review.
9. Analyzed price categories, discounts, and recent-sales indicators.
10. Created automated data quality checks.
11. Exported the cleaned dataset and quality reports.

## Key Results
- Original records: 3,986
- Records after duplicate removal: 3,777
- Exact duplicate rows removed: 209
- Missing product names after fallback: 0
- Missing or invalid prices: 0
- Products priced above $500: 26
- Missing discounts: 1,518
- Missing recent-sales indicators: 2,425
- Automated validation checks passed: 5

## Business Insights
- The median product price was $16.10.
- The average product price was $41.17.
- Most products were priced below $100.
- Higher-priced products were flagged for review rather than automatically deleted.
- Missing discount and sales information was preserved rather than assumed to be zero.

## Project Outputs
- `ecommerce_cleaned.csv`
- `ecommerce_quality_report.csv`
- `ecommerce_project_summary.csv`

## Limitations
The dataset contains missing discount and sales information. The recent-sales values are estimates extracted from text labels, not verified lifetime sales. High-priced products may be legitimate and were retained.

## Future Improvements
- Add automated tests using pytest.
- Build a dashboard using Power BI or Tableau.
- Automate data quality checks for new incoming datasets.
- Add logging and exception handling.

## Data Source
Kaggle: E-commerce Data Shein
