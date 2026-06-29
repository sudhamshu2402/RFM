# RFM Customer Segmentation Analysis

This project performs **RFM (Recency, Frequency, Monetary) Analysis** on customer transaction data to segment a customer base into distinct groups. By understanding customer behavior, businesses can optimize marketing strategies, improve customer retention, and maximize customer lifetime value (CLV).

## 📊 Dataset Overview
The dataset used in this analysis contains transactional records with the following columns:
* Customer ID: Unique identifier for each customer.
* Order ID: Unique identifier for each transaction.
* Purchase Date: The date and time when the transaction occurred (used to calculate **Recency**).
* Transaction Amount: The monetary value of the purchase (used to calculate **Monetary**).
* Product Information: Details about the item(s) purchased (used for cohort/product-level deep dives).
* Location: The geographic location of the customer (used for regional segmentation).

## 💡 Methodology: What is RFM?
RFM is a behavioral segmentation technique based on three core metrics:
1.  Recency (R): How recently did the customer make a purchase? (Days since last purchase).
2.  Frequency (F): How often do they purchase? (Total number of unique orders).
3.  Monetary (M): How much money do they spend? (Total transaction amount).

### Scoring and Segmentation
* Customers are assigned a score from 1 to 5 (or 1 to 4) for each metric using quantiles.
* These scores are combined to create an RFM Segment (e.g., "555" represents the highest-value customers).
* Segments are then mapped to human-readable personas (e.g., Champions, Loyal Customers, At Risk, Hibernating).



## 🚀 Key Features & Extended Analysis
Beyond standard RFM calculation, this project leverages the full dataset to provide:
* Geographic Insights Analysis of where the highest-scoring RFM segments are located to help optimize regional marketing campaigns.
* Product Affinity Identification of which product categories are most popular among "Champions" versus "At Risk" customers.

## 🛠️ Tech Stack
* Language: Python
* Libraries: Pandas, NumPy, Matplotlib, Seaborn, (Add Scikit-Learn if you used K-Means clustering)

## 📈 Key Findings & Business Recommendations
* Champions : Reward them with early access to new products. They are likely located in *[Insert Top Location]*.
* Can't Lose Them : These were once loyal but haven't bought recently. Win them back with personalized renewal offers or surveys.
* New Customers : Welcome them with onboarding emails and first-purchase discount triggers.
