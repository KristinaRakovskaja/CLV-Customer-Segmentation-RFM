# Customer Segmentation & RFM Analysis

In a growing business, understanding customer behavior is critical to long-term success. This is where customer segmentation and RFM analysis come in. Customer segmentation involves grouping similar customers together so we can tailor strategies for each group. RFM (Recency, Frequency, Monetary) analysis evaluates customer shopping habits—how recently they purchased (Recency), how often they purchase (Frequency), and how much they spend (Monetary).

Using this approach helps identify your best customers, recognize those at risk of churning, and fine-tune marketing strategies to maximize impact. Ultimately, it allows businesses to deepen relationships and boost performance.

## Project Overview

For this project, I worked with an RFM dataset containing invoice data, including when customers made purchases, what they bought, how much they bought, and how much they spent. The goal was to segment customers based on their RFM scores, develop a dashboard to visualize these segments, uncover insights about their purchasing behavior, and provide tailored recommendations for each customer group.

## Business Questions

1. How do different customer segments perform, and where should we focus our attention?
2. What are actionable strategies for each segment to improve engagement?

## Data Preparation & Cleaning

I reviewed the rfm table to understand the available data and identify what was necessary for effective segmentation.

To improve the quality of the analysis, I performed the following data cleaning steps:

- **Removed rows with missing customer IDs**: These rows could not be linked to any customer and were irrelevant for segmentation.

- **Excluded rows with** `unit_price = 0` **and** `quantity = 0`: These likely represent returns or non-transactional records.

With the cleaned dataset, I wrote a SQL query to calculate RFM values and assign each customer to the appropriate segment.

You can view the query and a snapshot of results in this Google Sheet:
👉 [Customer Segmentation & RFM](https://docs.google.com/spreadsheets/d/1NVSXGdkA1BfJBzL0Wkp7vv0eExArgtQrauY7b--v4i8/edit?usp=sharing)

## Analysis & Dashboard 

Using the segmented customer data, I built a Power BI dashboard to give a clear overview of each group's performance and provide actionable insights.

The full version of the Power BI dashboard can be found in the attached files above.

![image](https://github.com/user-attachments/assets/4685f5db-f821-4ba1-9e12-5f70c64b6a94)

The customers were segmented into the following groups: Best Customers, Big spenders, Loyal Customers, At Risk, About to Sleep, Customer Needing Attention, Potential Customers, Hibernating, New Customers, and Lost Customers.

Let’s review each segment and the recommended strategy:

**Best Customers** - Our most valuable customers, who spent the most, bought recently and most often, for the data we can see that they generate the most of our revenue and have a high average monetary value. To continue to be our customers, we need to occasionally reward them for being our best customers.

**Big Spenders** - Customers who spend a lot of money per purchase but may not buy frequently. They have a high monetary value but lower frequency or recency. We can increase their lifetime value by encouraging them to shop more often or with tailored premium offers.

**Loyal Customers** - These customers buy from us frequently, showing strong brand loyalty. Even if their total spending isn't the highest, their consistent purchases are valuable. We should nurture them through loyalty programs and personalized communication.

**At Risk** – Previously active customers who haven’t purchased in a while. Their recency is low, though they may have been valuable in the past. We should re-engage them with win-back campaigns, discounts, or personalized messages.

**About to Sleep** –  Existing customers who haven’t made purchases in a long time and are near the verge of becoming lost customers. We need to give a push to them, offer valuable information about our brand, create the most relevant message for them, and offer our popular product to reconnect with them.

**Customers Needing Attention** – These customers used to buy fairly often or spend well, but haven't been active lately. With moderate frequency and monetary value, they are at risk of churning. We can create a limited-time offer for them to reactivate them by recommendation of past purchase, where we could expect them to buy more. 

**Potential Customers** – These customers have made a recent purchase but are not yet frequent buyers and have low overall spending. To nurture this segment, we should focus on building brand awareness through targeted marketing campaigns, educating them about our products and values, and encouraging repeat purchases with free trials or introductory offers.

**Hibernating** – Inactive customers who haven’t bought in a long time, didn’t spend much when they did, and ordered a small number of products. They’re unlikely to return without strong incentives. With these customers, we need subtle reminders of the brand and gradually increase more compelling offers if the initial reminder does not work. 

**New Customers** – Recently acquired customers with only one purchase and little spending. With these customers, we need to engage more as they could be our top customers in the future. We can create more personalized campaigns based on their last purchase, send more information about the brand, and offer discounts for their next purchases. 

**Lost Customers** – Previously valuable customers who haven’t bought for a very long time. Their chances of reactivation are very low. If attempts to re-engage don’t work, they can be excluded from marketing efforts to reduce costs.

## Key Insights & Recommendations

- **Best Customers** and **Big Spenders** together make up **25%** of our current customer base and generate the most revenue. To retain and further engage them, we should focus on personalized strategies such as targeted email campaigns, upselling and cross-selling based on past purchases, free trials or product discounts, VIP loyalty programs with rewards, and exclusive time-limited offers.

- **Loyal Customers** form the foundation of our business, representing **11%** of our current customer base. They purchase frequently and have a strong purchase history, making them essential for long-term retention. To keep them engaged, we should focus on upselling higher-value products, offering exclusive rewards, requesting reviews, and maintaining consistent communication.

- **At Risk**, **About to Sleep**, **Customers Needing Attention**, **Hibernating**, and **Lost Customers** together account for **50%** of our current customer base, indicating that half of our customers are showing signs of disengagement. This highlights customer retention as a growing concern. To address this, we should launch targeted re-engagement campaigns using personalized discounts, product recommendations based on past behavior, and tailored email marketing. Priority should be given to **Hibernating** customers to prevent permanent churn. For **Lost Customers**, if these strategies prove ineffective, it may be more efficient to shift focus toward higher-potential segments. Additionally, conducting surveys can help uncover the reasons behind their disengagement.

- **Potential Customers** make up **10%** of our current customer base and represent a strong growth opportunity. With the right engagement strategies—such as loyalty or reward programs, personalized product recommendations, and incentives for repeat purchases—we can effectively guide them toward becoming **Loyal Customers**.

- **New Customers** make up only **3%** of our current customer base, indicating weak or insufficient customer acquisition. This suggests that our marketing efforts may be underperforming in attracting new buyers. To improve acquisition, we should strengthen our marketing strategies, optimize the onboarding experience, and implement referral programs, introductory discounts, or personalized welcome campaigns.
