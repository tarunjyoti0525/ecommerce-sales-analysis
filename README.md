# E-commerce Sales Analysis

## Project Overview
This beginner data analytics project uses Python to explore e-commerce sales records and identify patterns in revenue, product performance, monthly sales, country-level sales, and customer purchasing behavior.

## Objectives
- Explore the dataset and understand its structure.
- Clean duplicate records and convert date columns to datetime.
- Validate the revenue values against quantity multiplied by price.
- Calculate key performance indicators (KPIs).
- Compare products by quantity sold and revenue generated.
- Analyze monthly revenue, country revenue, and customer revenue.
- Summarize findings and practical business recommendations.

## Tools Used
- Python
- Pandas
- Matplotlib
- Jupyter Notebook

## Dataset
The notebook uses `ecommerce_sales.csv`.

The original dataset contains 10,000 rows and 10 columns:
`invoice`, `stockcode`, `description`, `quantity`, `invoicedate`, `price`, `customer_id`, `country`, `revenue`, and `invoice_month`.

After removing one exact duplicate, the cleaned dataset contains 9,999 rows. The notebook reports no missing values and no remaining exact duplicate rows.

> Keep `ecommerce_sales.csv` in the same folder as the notebook. Before sharing the project, update the notebook's CSV-loading line to use a relative path, such as `pd.read_csv("ecommerce_sales.csv")`, instead of a computer-specific `D:\ecommerce_project\...` path.

## Analysis Performed
1. Data exploration
2. Data cleaning and date conversion
3. Revenue validation
4. KPI calculation
5. Product performance analysis
6. Monthly revenue analysis
7. Country-wise revenue analysis
8. Customer analysis
9. Business insights and recommendations

## Key Results
The notebook reports the following results:

| KPI | Result |
|---|---:|
| Total revenue | £216,741.81 |
| Total items sold | 130,957 |
| Total invoices | 6,379 |
| Total customers | 2,666 |
| Average order value | £33.98 |

Additional findings:
- `WORLD WAR 2 GLIDERS ASSTD DESIGNS` had the highest quantity sold, at 7,261 items.
- `JUMBO BAG RED RETROSPOT` generated the highest revenue among physical products, at £3,495.55 (excluding postage).
- November 2011 was the highest-revenue month, at £31,896.91.
- The United Kingdom generated £176,602.55, approximately 81.48% of total revenue.
- Customer ID `17450` had the highest customer revenue in the analyzed data, at £8,188.46.

## Visualizations
The notebook includes four charts:
- Monthly Revenue Trend
- Top 10 Products by Revenue
- Top 10 Countries by Revenue
- Top 10 Products by Quantity Sold

## How to Run
1. Install Python and Jupyter Notebook (or use Jupyter through Anaconda).
2. Install the required libraries if needed:
   ```bash
   pip install pandas matplotlib notebook
   ```
3. Place `Project 1.ipynb`, `ecommerce_sales.csv`, and this `README.md` in the same project folder.
4. Open the notebook in Jupyter.
5. Ensure the CSV-loading line uses the relative path `pd.read_csv("ecommerce_sales.csv")`.
6. Select **Kernel → Restart Kernel**, then **Run → Run All Cells**.

## Limitations
- The analysis covers only the records included in the supplied dataset; it may not represent the full business history.
- Revenue and invoice frequency alone do not establish profitability or customer loyalty.
- The analysis identifies patterns but does not prove why they occurred or forecast future sales.

## Future Improvements
- Add a reproducible relative file path and document the dataset source.
- Investigate cancellations, returns, and negative quantities if present in the full source data.
- Add profit or margin analysis if cost data becomes available.
- Explore customer segments and repeat-purchase behavior.
- Add a dashboard in Power BI or Tableau as a separate project extension.
