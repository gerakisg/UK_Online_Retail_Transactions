# **Retail Sales Analysis with Python and SQL - Using a real-world dataset**

## The dataset used in this project is the **[Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)**, licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
## Chen, D. (2015). Online Retail [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33.

## Open in Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gerakisg/UK_Online_Retail_Transactions/blob/main/Notebook.ipynb)


## This project explores and analyzes the **UK Online Retail Dataset**, a transactional dataset containing e-commerce sales for a UK-based online retailer (2010–2011).  
I use Python to clean the data, perform EDA, RFM customer segmentation with K-means, Market Basket Analysis with FP-Growth, then use SQL queries for further analysis.

The goal:  
- Clean and preprocess transactional data  
- Perform descriptive and diagnostic EDA  
- Analyze customer behavior with RFM segmentation
- Perform Market Basket Analysis
- Study product performance and returns  
- Combine SQL + Python workflows for realistic, reproducible analysis  

## Dataset Description
- **InvoiceNo** – Transaction ID (cancellations prefixed with “C”)  
- **StockCode** – Unique product identifier  
- **Description** – Item description if available 
- **Quantity** – Number of items purchased (negative = returns)  
- **InvoiceDate** – Date/time of transaction  
- **UnitPrice** – Price per item  
- **CustomerID** – Unique customer identifier
- **Country** – Customer’s country  

## Workflow & Analysis Highlights
1. **Data Cleaning & Preparation**
   - Remove duplicates, handle missing values  
   - Filter invalid values
   - Treat extreme values / outliers
   - Derived revenue

2. **Exploratory Data Analysis**
   - Feature correlations
   - Distribution visualizations
   - Time Series analysis
   - Customer and Revenue Trends   

3. **Customer Segmentation (RFM)**
   - Recency, Frequency, Monetary metrics per customer
   - Customer clustering with K-means
   - Per-category customer statistics
   - Interpretation of customer behaviour
   - Visualization in 3D and 2D PCA space  
   - Alternative more flexible method

4. **Market Basket Analysis**
   - Frequent itemset mining with FP-Growth
   - Per-customer category frequent item sets recommendation
   - Comparison and similarities between categories

5. **SQL Analysis**
   - Top products by revenue, quantity and unique transactions  
   - Top returned products by revenue, quantity and unique transactions
   - Most common faulty/damaged/thrown away items 
   - Country specific stats  
