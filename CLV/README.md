# Customer Lifetime Value Analysis 

Customer Lifetime Value (CLV) stands at the forefront of e-commerce analytics, serving as a crucial metric to gauge the long-term value of customer relationships. Recent scrutiny over Shopify's simplistic CLV formula has prompted a shift towards cohort analysis for more reliable insights. This adjustment responds to two key concerns raised by the manager: the need to include all website users, not just purchasers, and the preference for a 12-week cohort analysis to capture customer engagement dynamics more effectively. The ongoing refinement of CLV calculations underscores its indispensable role in shaping marketing strategies and business planning by providing a nuanced understanding of customer value over time.


# Main Analysis

**1. Weekly Average Revenue by Cohorts (USD)**

As the first step, you should write 1 or 2 queries to pull data on weekly revenue divided by registrations. Since in this particular site there is no concept of registration, we will simply use the first visit to our website as the registration date (registration cohort).

![image](https://github.com/user-attachments/assets/0793f2be-ca4e-4c79-96de-6f82d82d86ec)

#### INSIGHTS

◾ Users are most likely to make a purchase during the first week after registering.

◾ Average weekly purchases decline steadily over time, with a sharp drop after week 0, suggesting user engagement decreases quickly.

◾ After week 6, revenue stabilizes at a low level (around $0.02), indicating most users stop purchasing or only buy occasionally.

◾ Users who registered between November and mid-December show higher spending in their first week compared to those in later cohorts.

#### RECOMMENDATIONS

1️⃣ Implement re-engagement strategies such as email reminders, discounts, or loyalty programs to boost repeat purchases.

2️⃣ Focus marketing efforts on maintaining user engagement after their initial purchase.

**2. Cumulative Revenue by Cohorts (USD)**

In the upcoming chart, the revenue/registrations for a specific weekly cohort will be expressed as a cumulative sum. To construct this chart, the revenue from the previous week was simply added to the current week’s revenue.

![image](https://github.com/user-attachments/assets/d69c4be6-b6a1-42be-8545-e14e577e1cbb)

#### INSIGHTS

◾The November cohorts, particularly the November 8th cohort, showed strong long-term user value growth. Despite having only 16K registrations, this cohort delivered the highest long-term value. This raises the question: did we do something differently for this cohort?

◾In contrast, the December and January cohorts underperformed, generating less than $1 per user on average. This may be due to seasonal effects or changes in marketing strategy.

◾A clear pattern emerged: higher first-week purchases are associated with higher long-term value.

◾Revenue growth is strongest in the early weeks, dips to its lowest point by week 9, and then slightly recovers between weeks 10 and 12. This suggests declining repeat purchases and increasing churn over time.

◾Our Customer Lifetime Value (CLV) at week 12 is $1.56, while our Customer Acquisition Cost (CAC) is $2.00 — resulting in a loss of $0.43 per customer.

#### RECOMMENDATIONS

1️⃣ Develop strategies to extend customer spending beyond the initial weeks.

2️⃣ Analyze high-performing cohorts (e.g., Nov 8) to identify successful tactics.

3️⃣ Investigate underperforming cohorts to understand what went wrong or what could be improved.

**3. Revenue Prediction by Cohorts (USD)**

Next, the focus is on the **future and trying to predict the missing data**. In this case, missing data is the revenue we should expect from later-acquired user cohorts. For example, for users whose first session happened on `2021-01-24` week, we have only their first week revenue, which is 0.19$ per user who started their first session in this week. Though we are not sure what will happen in the next 12 weeks. For this, we will simply use the previously calculated Cumulative growth % and predict all 12 future weeks' values.

![image](https://github.com/user-attachments/assets/3234b0c4-b6eb-4f3a-a691-eecddd1608a3)

#### INSIGHTS

◾Users from the November and December 6th cohorts are expected to contribute more to revenue over the next 12 weeks.

◾In contrast, users from other cohorts show lower spending, possibly due to post-holiday seasonality, as people tend to spend less after Christmas and New Year.

◾The January 17th cohort appears to be an outlier with higher-than-expected performance. This raises the question: was there a specific campaign or event that drove this result?

#### RECOMMENDATIONS

1️⃣ Strengthen marketing efforts to maintain customer engagement over time.

2️⃣ Introduce targeted promotions to increase future spending, especially during lower-activity periods.


