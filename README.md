# Global-Electronics-Retail-Sales-2016-2021

## Background & Overview

**Nexora Electronics** is a fictitious global electronics retailer with operations spanning North America, Europe, and Australia. The company offers a diverse range of consumer electronics including computers, mobile devices, TVs, cameras, audio systems, home appliances, and entertainment products. Nexora’s omnichannel strategy allows it to sell products both through its e-commerce platforms and physical retail stores.

This project is built on six years of transaction-level data (from 2016 to 2021),sourced from Maven Analytics and includes multiple interconnected datasets, covering:

•	Sales and order transactions

•	Customer demographics

•	Product information

•	Store locations

•	Currency exchange rates

**The primary objective is to analyze sales performance to identify how different product categories generate value and what levers can realistically improve performance to help sales teams refine sales stratergies.**



## Data Structure and Overview

**Sales** - Fact table containing transaction-level records. Each row represents a specific order line, including order and delivery dates, quantity, unit price, and related foreign keys for customer, product, store, and currency.

**Products** - Dimension table listing product details, including product name, brand, category, sub-category, description, pricing, and lifecycle dates.

**Customers** - Dimension table with customer demographic information such as customer ID, name, birthdate, gender, and country.

**Stores** - Dimension table containing store-level attributes including store name, location (city, country), and a unique store identifier.

**Exchange_Rates** - Table containing historical currency exchange rates by date and currency code, used for converting transaction values to USD.







<img src="https://github.com/rutujads-1/Global-Electronics-Retail-Sales-2016-2021/blob/main/Images/ERD%20.jpg" alt="Sales Dashboard" width="900" />









## Executive Summary

Total Revenue for 2016 to 2020 was $55M with a profit of $26.6M  from 26K orders. **Revenue and order counts showed a parallel upward movement increasing Year over Year.** Both metrics **reached the peak in 2019** before falling sharply in 2020 owing to the pandemic. In 2020 revenue and order counts dropped sharply following a downward trend throughout the year.
 
Quarterly patterns reveal that each year till 2019, **revenue and order counts showed a decline in the first two quarters and a massive rise in the last two**. The slump in the first two quarters could be attributed to — and the year end rise could be attributed to holiday season surges. 

The major drivers of this seasonality trend were- computers, cameras and camcorders, cell phones and TV and Video.

Overall, regionally- United States,United Kingdom and Germany were the top 3 Revenue Contributors. Second in line to in-store US channels, the online channel generated a revenue of $ 11M.

Overall,in terms of average order value- it was comparable across regions.



<img width="575" alt="image" src="https://github.com/user-attachments/assets/0f498306-4ef2-4c83-80c0-c06569037237" />





## Insights Deep Dive

**Product Performance**

**Core Revenue Drivers**

1. Computers category is the primary driver, leading across revenue and order volume which indicates strong demand and high ticket value. Consumers buy them often and they are high cost items which explains the high revenue, order volume.

2. Home Appliances generate the second highest revenue, driven by high AOV than order volume which means consumers buy less but when they buy they spend high amounts per order as these products have high costs. 

3. Cameras & Camcorders, Cell Phones, and TV & Video operate in a similar revenue band after computers and home appliances.The items in these categories are bought often by consumers but are not high cost items in comparison to other countries thus generating less revenue despite more purchases.

**Volume Driven Categories**

1. Cell Phones, Music, Movies & Audiobooks, Audio, and Games & Toys generate the highest order volumes. Despite strong order volumes, apart from cell phones, other categories don't generate translate the order volume to revenue.

These categories would benefit from dynamic SKU planning aligned to demand cycles which would help optimise inventory. 


**Average Order Volume Dynamics**

1. Home Appliances have the highest AOV, followed by TV & Video, Computers, and Cameras & Camcorders, which cluster in a similar premium range. 

2. Cell Phones sit in the mid-range AOV, while Games & Toys have the lowest AOV overall as they have comparatively low priced and generate less orders.


Volume driven categories rely heavily on frequency and not basket size while lower volume but higher AOV categories compensate through pricing.


**Underperforming Categories**

1. Audio, Music, Movies & Audiobooks, and Games & Toys contribute the least revenue, despite relatively strong order volumes.

2. Home Appliances, Cameras & Camcorders, and TV & Video show low order volume, but this is expected given their premium nature.

**Profitability Context**

Profit margins are broadly similar across categories which means the differences in performance come from customer demand and pricing of the products. So product teams don't need to remove any product at this stage as all categories are profitable, but they serve different roles in the product portfolio. 


**Regional Analysis**

Regionally, across the 8 countries similar categories show the aforementioned patterns. 

United States drove the largest revenue and order count with the main drivers being Computers and Home Appliances. United Kingdom,Germany and Canada fell in the mid range in terms of revenue and order volume while Australia, Italy, Netherlands and France drove lowest revenue and order volume in a similar range. 



Overall, the categories can be divided based on order volume and revenue:

1. Computers- high order count and high Revenue

2. Home Appliances- high Revenue, low order count

3. Cell Phones- high order count, mid range Revenue

4. Cameras and camcorders- mid range revenue, low range order count

5. TV and Video- mid range revenue, low order count

6. Music Movies and Audio Books- high order count but low revenue

7. Audio- similar to the above category- high order count but low revenue

8. Games and Audio- low revenue, mid range order count


We need different sales stratergies across categories as each cluster contributes differently to overall performance. 


**Channel Analysis**

Revenue coming from sale of products in store is $44M through 20K orders while online sales generate $11M via 5K orders. The AOV is thus comparable across channels. 

Both channels are economically viable, but in-store performance is driven by higher transaction frequency rather than high spend per order. So online channels should complement in-store channels rather than replace them. 






## Questions to Stakeholders, Assumptions & Caveats


### Questions to Stakeholders before Progressing in the Project

1. Are there any discount strategies or promotional campaigns applied historically?
   
*The dataset only includes the product unit price, not actual sale prices or discounts.*

2. What defines a successful order — revenue volume, frequency, or customer retention?
   
*This would help refine KPIs and prioritize analysis dimensions accordingly.*

3. Do we want to track repeat customer behavior and long-term value?
   
*This may require additional data on customer retention, satisfaction, or loyalty programs.*

## Recommendations

1. The highest demand is in Q3 and Q4 across regions. Since customers buy home appliances less often but spend more when they do which is during Q3 and Q4, offering sensible bundles during peak seasons can encourage them to buy more in one go. Regionally, in regions like France and Netherlands stock those products that consumers are buying during those peak periods rather than bundling of products.

2. Cell phones- this category is majorly volume driven hence we should focus on SKUs that have high demand across years specific to regions and sell them more often and make them easy to buy with right add-ons. Categories like Touch Screen Phones and Smart phones & PDAs are the two that consistenly drive highest unit volumes should be focused on.

3. In low demand regions like France and Netherlands maintain all categories
  
 


### Assumptions

1. All sales are assumed to be at full unit price.
   
Since no discount, promotional, or negotiated prices are provided, revenue is calculated as:

Revenue = Quantity × Unit Price

2. Product cost and unit price are fixed over time.
   
There's no time-based fluctuation captured in product pricing.


### Caveats

1. Revenue is estimated using full Unit Prices without considering discounts, returns, or promotional pricing.

2. The analysis does not factor in currency exchange rate volatility over time — all revenue figures are calculated in USD using the provided static rates.












