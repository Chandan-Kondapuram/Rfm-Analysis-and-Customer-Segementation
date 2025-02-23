# Customer Segmentation Using RFM Analysis

## Project Overview
This project implements **RFM (Recency, Frequency, Monetary) Analysis** to segment customers based on their purchasing behavior. The goal is to identify high-value customers, potential loyalists, and at-risk customers to optimize marketing strategies and improve customer retention.

## What is RFM Analysis?
RFM analysis is a technique used in customer segmentation that considers three key factors:
- **Recency (R):** How recently a customer made a purchase.
- **Frequency (F):** How often a customer makes purchases.
- **Monetary (M):** How much a customer spends.

By analyzing these metrics, businesses can better understand their customers and personalize marketing strategies.

## Steps Performed

### 1. Data Preprocessing
- Loaded the dataset and cleaned missing values.
- Converted the `InvoiceDate` column to a datetime format.
- Created a new column `Total Spend` by multiplying `Quantity` and `UnitPrice`.

### 2. Calculating RFM Metrics
- **Recency:** Number of days since the last purchase.
- **Frequency:** Number of transactions per customer.
- **Monetary:** Total amount spent by each customer.

### 3. Assigning RFM Scores
- Used quantiles to assign scores from **1 to 5** for each RFM metric.
- Customers were categorized based on these scores:
  - **Recency:** More recent purchases get higher scores.
  - **Frequency & Monetary:** Higher values get better scores.

### 4. Customer Segmentation
Using RFM scores, customers were segmented into groups such as:
- **Best Customers** (High Recency, High Frequency, High Monetary)
- **Loyal Customers**
- **Potential Loyalists**
- **At Risk Customers**
- **Lost Customers**

### 5. Data Visualization
Several visualizations were created to gain insights into customer segmentation:
- **Customer Segmentation Count:** A bar chart showing the distribution of customer segments.
- **RFM Correlation Heatmap:** Displays the relationship between Recency, Frequency, and Monetary metrics.
- **Monetary vs Frequency Scatter Plot:** Helps identify high-value and repeat customers.
- **Boxplots for RFM Metrics:** Compare Recency, Frequency, and Monetary distributions across segments.

## Key Findings
- **Best Customers** are frequent buyers with high spending.
- **At Risk & Lost Customers** require targeted marketing strategies for re-engagement.
- **RFM segmentation provides valuable insights** into customer purchasing behavior.

## Future Enhancements
- Implement **K-Means Clustering** to compare with RFM-based segmentation.
- Use **machine learning models** for automated segmentation.
- Develop an interactive **dashboard** for real-time customer insights.



