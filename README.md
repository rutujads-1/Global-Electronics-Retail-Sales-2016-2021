# Global-Electronics-Retail-Sales-2016-2021

## Background & Overview

**Nexora Electronics** is a fictitious global electronics retailer with operations spanning North America, Europe, and Australia. The company offers a diverse range of consumer electronics including computers, mobile devices, TVs, cameras, audio systems, home appliances, and entertainment products. Nexora’s omnichannel strategy allows it to sell products both through its e-commerce platforms and physical retail stores.

This project is built on six years of transaction-level data (from 2016 to 2021),sourced from Maven Analytics and includes multiple interconnected datasets, covering:

•	Sales and order transactions

•	Customer demographics

•	Product information

•	Store locations

•	Currency exchange rates

The primary objective is to analyze historical sales performance and customer behavior to uncover actionable insights that can drive data-informed decision-making across departments.

Key Business Questions Answered:

*• What types of products does the company sell, and where are customers located?*

*•	Are there any seasonal patterns or trends in order volume or revenue?*

*•	How long is the average delivery time in days? Has that changed over time?*

*•	Is there a difference in average order value (AOV) for online vs. in-store sales?*

This dashboard and analysis are designed to assist cross-functional teams including:

**•	Sales & Regional Management** – to evaluate market performance and guide regional revenue strategies.

**•	Marketing & Customer Insights** – to understand customer trends and optimize targeting efforts.

**•	Retail Operations** – to compare online vs. in-store performance and enhance operational efficiency.

**•	Executive Leadership** – to support data-driven strategic decision-making through performance insights.

**Key Performance Indicators (KPIs) Tracked:**

•	Total Revenue

•	Order Volume

•	Average Order Value (AOV)

•	Distinct & New Customer Counts

•	Average Delivery Time

•	Channel-wise and Region-wise Revenue Trends


## Data Structure and Overview

**Sales** - Fact table containing transaction-level records. Each row represents a specific order line, including order and delivery dates, quantity, unit price, and related foreign keys for customer, product, store, and currency.

**Products** - Dimension table listing product details, including product name, brand, category, sub-category, description, pricing, and lifecycle dates.

**Customers** - Dimension table with customer demographic information such as customer ID, name, birthdate, gender, and country.

**Stores** - Dimension table containing store-level attributes including store name, location (city, country), and a unique store identifier.

**Exchange_Rates** - Table containing historical currency exchange rates by date and currency code, used for converting transaction values to USD.








![image](https://github.com/user-attachments/assets/e0bddba8-aac0-4cef-813c-1526a140469d)








## Executive Summary

From 2016 to 2021, the company generated a total revenue of $55.76M total gross profit of $32.66M from over 63,000 orders, with an Average Order Value (AOV) of $886.60.
Revenue grew steadily from 2016 to 2019, peaking at $18.26M just before the pandemic. However, sales declined sharply in 2020 to $9.29M, and dropped further to $1.04M in 2021, highlighting the significant impact of the pandemic on performance.

Order volume followed a similar trend, reaching a high of 68440 orders in 2019, before falling to 34463 in 2020, and just over 3797 orders in 2021 so far.

Overall, in-store revenue surpassed online revenue by $33M, indicating continued customer preference for physical retail during the period analysed.

Regionally, the United States, United Kingdom, Germany, Canada, and Australia were the top five revenue-generating countries, while Italy, the Netherlands, and France contributed the least to overall revenue.

Among all brands, Contoso consistently recorded the highest order volume, reflecting strong brand preference.


## Insights Deep Dive

*Are there any seasonal patterns or trends for order volume or revenue?*

**Revenue Trends**




<img width="235" alt="image" src="https://github.com/user-attachments/assets/ed61e684-6a1f-4d22-b03b-d15c69b7b4ab" />









Between 2016 and 2021, the company experienced strong growth followed by a sharp decline, reflecting changing market dynamics and likely external disruptions.

•	Annual Revenue Trends:

o	2016: $6.95M

o	2017: $7.42M

o	2018: $12.79M

o	2019: $18.26M (Peak Year)

o	2020: $9.29M (Nearly 50% decline from 2019)

o	2021: $1.04M (Significant drop post-pandemic)


Quarterly Revenue Trends & Key Observations:

**2016**

•	Q1 to Q2: Decline ($1.88M → $1.23M)

•	Q2 to Q3: Growth ($1.23M → $1.57M)

•	Q3 to Q4: Continued Growth ($1.57M → $2.27M)

Steady recovery through the year after a weak Q2.

**2017**

•	Q1 to Q2: Drop ($1.75M → $1.31M)

•	Q2 to Q3: Modest Growth ($1.31M → $1.79M)

•	Q3 to Q4: Strong Finish ($1.79M → $2.57M)

Despite a sluggish mid-year, Q4 helped end the year on a positive note.

**2018**

•	Q1 to Q2: Decline ($2.70M → $2.12M)

•	Q2 to Q3: Growth ($2.12M → $3.17M)

•	Q3 to Q4: Continued Growth ($3.17M → $4.80M)

Strong upward momentum in H2.

**2019**

•	Q1 to Q2: Decline ($4.89M → $3.15M)

•	Q2 to Q3: Growth ($3.15M → $4.46M)

•	Q3 to Q4: Further Growth ($4.46M → $5.77M)

Despite a Q2 dip, 2019 delivered the highest revenue overall.

**2020**

•	Q1 to Q2: Sharp Decline ($4.97M → $1.86M)

•	Q2 to Q3: Further Drop ($1.86M → $1.31M)

•	Q3 to Q4: Continued Drop ($1.31M → $1.15M)

Heavily impacted by the pandemic, showing a consistent downward trend.

**2021 (Partial)**

•	Jan to Feb: Slight Recovery ($513K → $526K)

While overall revenue remains low, early 2021 shows minor improvement month over month.

Across all years from 2016 to 2019, a clear quarterly pattern emerges in revenue performance:

•	Q1 to Q2: Revenue consistently declines, likely due to a post-holiday sales slump or slow seasonal demand.

•	Q2 to Q3: Revenue begins to recover, signalling a rebound in consumer activity.

•	Q3 to Q4: The company experiences significant growth, possibly driven by holiday-season promotions and end-of-year sales.

This consistent pattern suggests that the business is seasonally influenced, with stronger revenue performance in the second half of the year.

**Order Volume Trends**

Order Volume Trend Analysis (2016–2021)






<img width="236" alt="image" src="https://github.com/user-attachments/assets/b96f5fe6-360b-4744-8fc3-ebbf6aab3501" />











**Annual Order Volumes**

•	2016: 21761 products sold

•	2017: 24798 products sold

•	2018: 44498 products sold

•	2019: 68440 products sold (Peak year)

•	2020: 34463 products sold

•	2021: 3793 products sold

Order volumes steadily increased from 2016 to 2019, peaking in 2019. However, a sharp decline followed in 2020 due to the pandemic, continuing into 2021.

**Quarterly Trends and Seasonal Patterns**

**2016**

•	Q1 to Q2: Decline (5687 → 3836)

•	Q2 to Q3: Growth (3836→ 5068)

•	Q3 to Q4: Further Growth (5068 → 7170)

**2017**

•	Q1 to Q2: Decline (5805 → 4065)

•	Q2 to Q3: Growth (4065 → 5897)

•	Q3 to Q4: Further Growth (5897 → 9031)

**2018**

•	Q1 to Q2: Slight Decline (8705 → 7450)

•	Q2 to Q3: Growth (7450 → 11317)

•	Q3 to Q4: Further Growth (11317→ 17026)

**2019**

•	Q1 to Q2: Decline (17328 → 12025)

•	Q2 to Q3: Growth (12025 → 17287)

•	Q3 to Q4: Further Growth (17287→ 21800)

From 2016 to 2019, a clear seasonal pattern is observed:

•	Q1 to Q2: Decline in orders

•	Q2 to Q3: Recovery

•	Q3 to Q4: Continued growth

From 2016 to 2019, the business consistently followed a seasonal pattern in order volumes:

•	Q1 to Q2: A decline in order volume is observed across all years — possibly due to a slowdown after the holiday season.

•	Q2 to Q3: Orders begin to recover, showing strong growth as consumer demand picks up mid-year.

•	Q3 to Q4: Order volumes continue to grow, peaking during the holiday and end-of-year period.

This trend mirrors the revenue trend, suggesting that both metrics are influenced by seasonal consumer behaviour and retail cycles. This pattern suggests mid-to-late-year surges in demand, likely tied to seasonal promotions and holidays.

**Pandemic Impact**

**2020**

•	Q1 to Q2: Sharp Decline (18483 → 6688)

•	Q2 to Q3: Further Drop (6688→ 4795)

•	Q3 to Q4: Slight Decline (4795→ 4497)

**2021 (Partial)**

•	Jan to Feb: Slight Decline (1848 → 1949)

The post-pandemic years broke the seasonal pattern, with continuous declines in order volume throughout the year, reflecting global disruptions and decreased consumer activity.


*What types of Products does the Company Sell?*

The company offers a diverse range of products across categories such as **Computers, Home Appliances, Cameras & Camcorders, Cell Phones, TV & Audio, Music, Movies & Audiobooks, and Games & Toys**.

**Product Performance**

*The top performing categories by revenue are Computers, Home Appliances, Cameras and Camcorders, Cell Phones, and TV & Video.*

•	**Computers** showed a strong upward trend from 2016 ($1,496,820) to 2017 ($2,228,431.91), with a steady rise peaking in 2019 at $6,958,430.89. Revenue declined from 2019 through the pandemic, falling to $445,745.65 in 2021.

•	Within the Computers category,**Desktops** emerged as the highest revenue-generating subcategory. The leading contributors to this segment were the brands **Adventure Works and Wide World Importers**, which together drove most of the desktop revenue.

•	**Home Appliances** maintained a steady trend between 2016 ($2,010,476.12) and 2017 ($2,065,843.64), then rose to $2,834,487.33 in 2018 before declining post-2019 to $77,082.06 in 2021. 

•	Within the Home Appliances category, **Water Heaters** generated the highest revenue. The brand **Contoso** was the top contributor, driving the majority of revenue in this product line.

•	**Cameras and Camcorders** dipped slightly in 2017 ($721,318.38) after 2016 ($946,180.01), then increased steadily until a 2019 peak of $2,260,124.97. Revenues dropped after that, reaching $129,196.99 in 2021.

•	Within the Cameras & Camcorders category, **Camcorders** were the top revenue-generating product type. The brand **Fabrikam** led this segment, contributing the highest revenue among all brands.

•	**Cell Phones** followed a consistent rise from 2016 ($429,497.27) to a peak of $2,311,957.73 in 2019, before dropping to $159,454.04 in 2021.

•	Within the Cell Phones category, **Touch Screen Phones** accounted for the highest revenue. The brand **The Phone Company** was the top performer in this segment, generating the most revenue.

•	**TV & Video** saw an early decline from 2016 ($1,266,376.10) to 2017 ($819,355.08), then rose through 2019 ($1,664,768.48), before falling again to $101,951.88 in 2021.

•	Within the TV & Video category, **Televisions** were the highest revenue-generating product type. The brand **Adventure Works** led this category, contributing the most revenue from television sales.

*In terms of order volume, the top 5 categories are: Computers, Cell Phones, Music, Movies & Audio Books, Audio, and Games & Toys.*

•	Computers increased from 3435 items in 2016 to a peak of 16203 in 2019, before declining to 7941 in 2020 and 982 in 2021.

•	**Cell Phones** rose from 2277 in 2016 to 11728 in 2019, then dropped to 6409 in 2020 and to 738 in 2021 so far.

•	**Music, Movies & Audio Books** began at 3607 in 2016, peaked at 9494 in 2019, and fell to 5019 by 2020 and is at 587 in 2021.

•	**Audio** rose from 2492 items in 2016 to 7959 in 2019, declining to 3356 in 2020 and finally is at 323.

•	**Games & Toys** started at 1710 items in 2016, peaked at 9278 in 2019, and fell to 4956 in 2020 and is at 455 in 2021.

Total orders from in-store channels were 37,776, while online orders accounted for 10,126, confirming stronger in-store performance during the years analysed.

Among individual products:

•	**Adventure Works Desktop PC2.30 MD230 Black** was the most ordered product in terms of order counts.

•	**WWI Desktop PC2.33 X2330 Black** was the highest revenue-generating product


*Where are the Customers located?*

The comapany's customer base spans three continents—**Australia, Europe, and North America**—covering eight countries: **Australia(780 customers), Canada(1179), France(438), Germany(1150), Italy(530), the Netherlands(534), the United Kingdom(1570), and the United States(5706)**.

*Customer and Regional Analysis*

**Revenue by Region**

The top five regions by revenue are: **United States, United Kingdom, Germany, Canada, and Australia**.

**United States**

Revenue rose from $2.8M in 2016 to a peak of $7.85M in 2019, followed by a decline to $464K in 2021.

In 2016, there were 1,040 new customers regionally, but this number declined to 940 in 2017. The trend reversed in 2018, with a rise to 1,172 new customers. However, 2019 saw a slight decline to 1,035, followed by a significant drop in 2020 to 291. By 2021, only 20 new customers were added, highlighting a sharp downturn likely influenced by external factors such as the pandemic.

**United Kingdom**

Revenue increased steadily from $871K in 2016 to a peak of $1.7M in 2019, then declined to $71.5K by 2021.

In the United Kingdom, there were 358 new customers in 2016, which declined to 288 in 2017. The number rose slightly in 2018 to 322 but dropped again to 226 in 2019. The downward trend continued in 2020 with 86 new customers, reaching just 4 in 2021, indicating a sharp decline in new customer acquisition over time.

**Germany**

Revenue grew from $572K in 2016 to $1.5M in 2019, then declined to $60K in 2021.

In 2016, Germany had 179 new customers, which saw a slight drop to 176 in 2017. The number then increased to 244 in 2018 and remained relatively stable in 2019 with 243. However, 2020 marked a significant decline to 60, and by 2021, the number dropped further to just 3 new customers, reflecting a sharp slowdown in customer acquisition post-2019.

**Canada**

Revenue increased from $509K in 2016 to $1.13M in 2019, then fell to $68.5K in 2021.

In 2016, Canada saw 199 new customers, which declined to 176 in 2017. The number rebounded in 2018 with 232 new customers, followed by a slight dip to 228 in 2019. A significant decline occurred in 2020, with the number falling to 91, and further dropping to just 5 new customers in 2021.

**Australia**

Revenue rose from $274K in 2016 to $689K in 2019, before declining to $24.8K in 2021.

In 2016, Australia had 97 new customers, followed closely by 96 in 2017. The numbers increased to 163 in 2018 and peaked at 171 in 2019. A downward trend began in 2020, with new customers dropping to 71, and further to just 7 in 2021.

**Average Order Value (AOV) by region**

The top five countries by AOV were: **Italy, Australia, Germany, United States, and France**.

•	**Italy**: AOV ranged from $757.6 (2021) to $1,095.2 (2016), showing fluctuations but a general decline over time.

•	**Australia**: Peaked at $1,078 (2016), declined to $671.4 (2021).

•	**Germany**: Dropped early but saw a spike to $1,117.5 in 2021.

•	**United States**: Gradual decline from $1,016.7 in 2016 to $844.1 in 2020, with a slight rebound in 2021.

•	**France**: AOV peaked at $957.8 in 2020 but dropped sharply to $639 in 2021.

*Top Customers*

•	Highest Revenue Generated: **Matthew Flemming (United States)**

•	Highest AOV: **Kian Sims (United Kingdom)**

•	Most Orders Placed (in terms of both volume and order counts): **Gaspare Trevisan (Italy)**

*Is there a difference in average order value (AOV) for online vs. in-store sales?*

**Online Trends**

*Revenue*

Online revenue showed steady growth from $1.17M in 2016 to a peak of $3.91M in 2019. Afterward, it declined to $2.07M in 2020 and $285K in 2021.

*AOV (Average Order Value)*

Online AOV started at $1,007.2 in 2016, gradually declining to $832.7 in 2019. It remained relatively flat in 2020 ($832.3) and slightly increased to $858.2 in 2021.

*Customer Trend*

The number of new online customers increased from 431 in 2016 to 656 in 2018. It then declined slightly to 625 in 2019, followed by a sharper drop to 219 in 2020 and just 20 in 2021.

 **In-Store Trends**
 
*Revenue*

In-store revenue began at $5.78M in 2016, steadily increasing to a peak of $14.36M in 2019. Revenue declined to $7.22M in 2020, and further to $753K in 2021.

*AOV (Average Order Value)*

In-store AOV declined year-over-year from $1,005.8 in 2016 to $848.6 in 2019 and reached $857.2 in 2021 after a minor dip in 2020 ($846.1).

*Customer Trend*

New in-store customers totalled 2,130 in 2016, declining to 1,898 in 2017. The number rose again to 2,448 in 2018, then dipped to 2,207 in 2019. A significant drop followed in 2020 with just 728 new customers, and the figure currently stands at 47 in 2021.

**Key Insight**

Overall, the Average Order Value (AOV) for in-store purchases ($892) is comparable to that of online purchases ($866.3). While the order volume is significantly higher in stores (49,719 vs. 13,165 online), the data suggests that online customers shop less frequently but tend to place higher-value orders.

*How long is the average delivery time in days? Has that changed over time?*

**Average Delivery Time**

The overall average delivery time from 2016–2021 is **4.53 days**.

It has steadily declined:

•	7.29 days in 2016

•	5.19 in 2017

•	4.31 in 2018

•	4.08 in 2019

•	4.03 in 2020

•	3.85 in 2021

*There are currently 50K undelivered orders in the system, which may impact future delivery metrics*.

## Recommendations 


## Questions to Stakeholders, Assumptions & Caveats









