# Customer-Recommender-System

**DATA OVERVIEW**
For this project I worked with a transactional dataset which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered e-commerce store. 
The dataset includes transaction details with unique invoice and product IDs, product descriptions, quantities, prices, transaction dates, customer IDs, and customer locations, where each transaction and product are uniquely identified, and cancellations are flagged by a specific code in the InvoiceNo (If the Invoice No. starts with a ‘C’ it indicates a cancellation).
This dataset consists of over 3823 customers from 38 different countries, and deals with 4070 products.

**OBJECTIVE:** 
The goal of segmenting customers is to identify distinct groups within a larger customer base. Each group, or cluster, is composed of customers who share similar purchasing behaviors. By understanding these patterns, businesses can tailor their marketing efforts more effectively.

**METHOD:** 
Using techniques like PCA and KMeans clustering, RFM analysis segmented customers into four distinct clusters based on similar purchasing patterns for better cluster exclusive marketing strategies.
Evaluated key metrics for each cluster, such as;    
**Average Sales per Customer** and **Average Sales per Invoice** to determine spending patterns.
**Average Recency** and **Average Frequency** to evaluate customer engagement.
**Average Number of Invoices per Customer** to assess purchasing behavior.

**PURPOSE:** 
After segmenting customers, market basket analysis (usinf FP-Growth) is used to uncover associations between different products within each cluster. This helps in understanding which products are frequently bought together by specific customer segments.
For example, if Cluster 2 frequently buys product A with product B, a targeted cross-sell campaign can be designed for customers in this cluster, offering discounts or promotions on product B when they purchase product A.

**CONCLUSION**
1. The k-mean cluster helped to group the customers into 4 categories. 
- Cluster 1 is the most valuable cluster, despite its small size, contributing the most to total sales.
- Cluster 0 and Cluster 2 represent a large number of customers, but they have very low sales contributions.
- Cluster 3 shows potential due to the high number of invoices per customer but has lower total sales compared to Cluster 1.
Understanding these clusters can help in tailoring marketing strategies, such as focusing on retention for Cluster 1 and re-engagement for Cluster 2.

2. The market basket analysis helped us to build association rules between antecedents and consequents based on lift, confidence and support (as displayed previously) for better cross-sell/up-sell strategies to drive more revenue for the company. 



