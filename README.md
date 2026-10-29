# Sales Performance & Target Achievement Dashboard

Beginner-friendly Power BI portfolio project.

## Files
- `sales.csv` — 500 sales/order rows
- `customers.csv` — 100 customer records
- `products.csv` — 12 products
- `targets.csv` — monthly sales targets by region
- `DAX_Measures.txt` — suggested measures and model relationships

## Data note
All records are synthetic sample data generated for learning and portfolio practice; they are not real company or customer data.

## Import
In Power BI Desktop, use Home > Get data > Text/CSV to import all four CSV files.

## Suggested dashboard
- Cards: Total Sales, Total Profit, Total Orders, Target Achievement %
- Column chart: Sales by Category
- Line chart: Sales by Month (use DateTable[YearMonth])
- Bar chart: Top 5 Products by Total Sales
- Bar chart: Sales by Region
- Gauge: Total Sales vs Sales Target
- Slicers: Date, Region, Category, CustomerSegment

## Relationships
- sales[CustomerID] to customers[CustomerID]
- sales[ProductID] to products[ProductID]
- DateTable[Date] to sales[OrderDate]
Use the DAX guide for target measures. For a first simple version, you can build visuals with Total Sales and Total Profit before adding target measures.
