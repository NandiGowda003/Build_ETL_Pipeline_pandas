# Build_ETL_Pipeline_pandas
 Walmart Holiday Supply &amp; Demand Analysis

## Overview
This project analyzes Walmart grocery sales around major U.S. holidays (Super Bowl, Labor Day, Thanksgiving, Christmas).  
The goal is to understand supply and demand fluctuations and provide a foundation for forecasting.

## Tech Stack
- **Python 3.x**
- **Pandas** for ETL and data analysis
- **PostgreSQL** as the source database
- **Matplotlib / Seaborn** for visualization (optional)

## Data Sources
- **grocery_sales (PostgreSQL table)**: contains product, store, date, and sales metrics.
- **Complementary data**: holiday calendar and external demand indicators.

## ETL Pipeline
1. **Extract**
   - Connect to PostgreSQL
   - Query grocery_sales and complementary datasets
2. **Transform**
   - Clean missing values
   - Aggregate sales by date, store, and product
   - Tag records with holiday flags
   - Compute demand spikes vs baseline
3. **Load**
   - Save transformed data into CSV/Parquet for analysis
   - Optionally load into a data warehouse/lake

## Validation
- validate the ETL function 
