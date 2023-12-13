**ML model used in CUSTOMER PERSONALITY ANALYSIS**

Customer Personality Analysis involves conducting a comprehensive examination of an organization's preferred client. This analysis aids in enhancing a business's comprehension of its customers, enabling them to adapt their products to cater to the distinct requirements, behaviors, and concerns of diverse customer groups. By conducting a Customer Personality Analysis, businesses can refine their products to align with the needs of specific customer segments. 

For instance, rather than investing resources in promoting a new product to every customer in their database, a company can identify the customer segment that is most likely to purchase the product and focus their marketing efforts exclusively on that particular segment.
Here we quantify customer behavior more effectively. During marketing campaigns, it is not advisable to contact all customers with the same level of effort. Direct marketing segmentation involves grouping customers into different segments to analyze their profitability accordingly.

We will utilize the BG/NBD and Gamma-Gamma models in this project. 

**BG/NBD:** This model can predict repeat visits by customers and helps understand whether a customer is likely to return.
**Gamma-Gamma:** This model forecasts the average amount of money a customer is expected to generate in a given time period.

**Data Collection:**

Gather relevant customer transaction data, including purchase dates, purchase amounts, and customer identifiers. Ensure the data is clean and free from errors or duplicates.

_**RFM Calculation:**_
Calculate the Recency (R) of each customer by determining the time elapsed since their last purchase. Calculate the Frequency (F) by counting the number of purchases made by each customer within a specific time period. Calculate the Monetary Value (M) by summing up the total purchase amounts for each customer within the same time period.

_**RFM Score Calculation:**_
Assign a score to each customer for Recency, Frequency, and Monetary Value based on appropriate quantiles or percentiles (e.g., 1 to 5 scale). Combine the three individual scores to create an RFM score (e.g., R=3, F=4, M=5 -> RFM Score = 345).

_**Customer Segmentation (using RFM):**_
Group customers based on their RFM scores into different segments (e.g., "Champions," "Loyal but Churning," "Potential Loyalists," etc.). Analyze the characteristics and behaviors of each segment to understand their value to the business.

_**CLTV Calculation:**_
Use predictive modeling techniques (e.g., regression, machine learning) to estimate the Customer Lifetime Value (CLTV) for each customer. Take into account factors like customer acquisition cost, retention rate, and average customer spend to calculate CLTV.

_**Customer Segmentation (using CLTV):**_
Segment customers based on their CLTV predictions into groups (e.g., "VIP Customers," "Acquisition Testing," etc.). Determine the long-term value of each segment to the business.

_**Actionable Insights:**_
Analyze the results and identify actionable insights for each customer segment. Develop targeted marketing strategies, personalized offers, and retention efforts for high-value segments to maximize their potential.

**RF Scores as Segments:**

![image](https://github.com/veera212/customer-personality-analysis/assets/110824377/d1ce68bb-7dc3-4599-b5af-872fbc64db2c)
![image](https://github.com/veera212/customer-personality-analysis/assets/110824377/92a0297b-d6df-4f63-bbf0-7f7f9b5a62ef)

**SYSTEM ARCHITECTURE:**

![image](https://github.com/veera212/customer-personality-analysis/assets/110824377/f4e35cbd-a1a9-4b95-a327-7ba0c9a6a223)

**Conclusion:**
We can see that the segments with the highest CLTV values are the Potential Loyalists, followed just after by the At Risk and Loyal Customers. We can use our new RFM segmentation along the CLTV to develop a classification model and determine which customers are most likely to be receptive to our next promotional marketing campaign.
