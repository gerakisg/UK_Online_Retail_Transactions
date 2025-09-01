# **Retail Sales Analysis with Python and SQL - Using a real-world dataset**

## The dataset used in this project is the **[Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)**, licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
## Chen, D. (2015). Online Retail [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33.

## Open in Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gerakisg/UK_Online_Retail_Transactions/blob/main/UK_Online_Retail_Transactions.ipynb)


## This project explores and analyzes the **UK Online Retail Dataset**, a transactional dataset containing e-commerce sales for a UK-based online retailer (2010–2011).  
I use Python to clean the data, perform EDA, RFM analysis, Basket Analysis with FP-Growth, then create a database and use SQL to query it.

The goal:  
- Clean and preprocess transactional data  
- Perform descriptive and diagnostic EDA  
- Analyze customer behavior (RFM segmentation)  
- Study product performance and returns  
- Combine SQL + Python workflows for realistic, reproducible analysis  

## Dataset Description
- **InvoiceNo** – Transaction ID (cancellations prefixed with “C”)  
- **StockCode** – Unique product identifier  
- **Description** – Item description (may contain missing values)  
- **Quantity** – Number of items purchased (negative = returns)  
- **InvoiceDate** – Date/time of transaction  
- **UnitPrice** – Price per item (GBP)  
- **CustomerID** – Unique customer identifier (may be null)  
- **Country** – Customer’s country  

## Workflow & Analysis Highlights
1. **Data Cleaning & Preparation**
   - Removed duplicates, handled missing values  
   - Filtered invalid values
   - Derived revenue

2. **Univariate & Bivariate Analysis**
   - Revenue trends by month, day of week, and hour
   - Customer purchasing behavior   

3. **Visualizations**
   - Boxplots (zoomed with percentiles, annotated values)  
   - Transactions and Revenue time series  

4. **Customer Segmentation (RFM)**
   - Recency, Frequency, Monetary metrics per customer  
   - Segmentation into `Top 5%`, `Top 20%`, `Top 50%`, and `Below Average`  
   - Segment-level summary (mean, median, revenue share %)  


5. **SQL Analysis**
   - Top products by revenue, returns, and unique invoices  
   - Customer & product cancellation correlations
   - Most common faulty/damaged/thrown away items 
   - Country specific stats  
