# Global-Electronics-Retail-Sales-2016-2021

## Background & Overview

**Nexora Electronics** is a fictitious global electronics retailer with operations spanning North America, Europe, and Australia. The company offers a diverse range of consumer electronics spread across 8 categories- Computers, Cell phones, TV and Video, Home Appliances, Music Movies and Audio Books, Audio, Cameras and camcorders, Games and Toys. Nexora’s omnichannel strategy allows it to sell products both through its e-commerce platforms and physical retail stores which are present in 8 countries- United States, United Kingdom, Germany, Australia, Canada, France, Italy and Netherlands.

This project is built on data that has six years of transaction-level  (from 2016 to 2021) includes multiple interconnected datasets, of which four years (2016-2019) are used for the purpose of this analysis, covering:

•	Sales and order transactions

•	Customer demographics

•	Product information

•	Store locations

•	Currency exchange rates



**The primary objective is to analyse sales performance across regions and categories and help sales teams device stratergies to harness areas of revenue growth.**



## Data Structure and Overview

**Sales** - Fact table containing transaction-level records. Each row represents a specific order line, including order and delivery dates, quantity, unit price, and related foreign keys for customer, product, store, and currency.

**Products** - Dimension table listing product details, including product name, brand, category, sub-category, description, pricing, and lifecycle dates.

**Customers** - Dimension table with customer demographic information such as customer ID, name, birthdate, gender, and country.

**Stores** - Dimension table containing store-level attributes including store name, location (city, country), and a unique store identifier.

**Exchange_Rates** - Table containing historical currency exchange rates by date and currency code, used for converting transaction values to USD.







<img src="https://github.com/rutujads-1/Global-Electronics-Retail-Sales-2016-2021/blob/main/Images/ERD%20.jpg" alt="Sales Dashboard" width="900" />









## Executive Summary

<p align="center">
  <img src="images/Exec page_trend.png" width="45%" />
</p>


<p align="center">
  <img src="images/repeat_purchases.png" width="45%" />
  <img src="images/customer_frequency.png" width="45%" />
</p>


The business generated a total revenue of $45M through 21K orders with a profit of ~ $27M in the years 2016 to 2019.

**Revenue and order volume showed a parallel upward trend till 2019. Over the years a quarterly trend emerged, where revenue and growth showed a decline from Q1 to Q2 and then an increase from Q3 to Q4. This pattern can be explained by the end of year festive surges.** 

The **major drivers** of the seasonality trend were- **computers, cameras and camcorders, cell phones and TV and Video**. 

Overall, computers were the major contributor in revenue and order volume. Games and Toys were the least contributors to revenue while TV and Video category drove the least orders. Profit margins were comparable across product categories which indicates performance is driven by revenue, order volume or Average Order Value(AOV). 

Regionally, the **United States** contributed to nearly half of the total revenue while countries like France earned the lowest revenue but the AOV was comparable across the countries which indicates that differences in order volume led to the differences in performance. 

Since the United States drove a revenue of ~19M which is almost half of the total revenue, the focus is on this market to identify levers of growth and areas of improvement. 



<img width="575" alt="image" src="https://github.com/user-attachments/assets/0f498306-4ef2-4c83-80c0-c06569037237" />





## Insights Deep Dive

### Product Performance In United States

Among the 8 product categories, different categories added different value in terms of the metrics- revenue and order volume. Top 3 products in terms of revenue were- Computers, Home Appliances and Cameras and camcorders. 

In terms of order volume the  top 3 products were- computers, cell phones and Music Movies and Audio Books. 

**Top Revenue generating products-**

Similar to the overall product trend, **computers are the most important category** in the United States driving a  total revenue of **$ 6M**  with **~4K orders**.
Within computers the desktop sub category drove revenue generating a total of $3M which is half of the total revenue the category generates while the accessory parts like printers, scanners and Fax generated the least revenue of $255K. Since this is a high performing category driven by desktops, during the peaks in Q4 high selling SKUs can be meaningfully bundled with accessory parts to increase basket value. 

Home Appliances is the second highest revenue generating with the highest AOV, which explains that this is a high priced category where users don’t buy frequently but spend heavy amounts per order. This category is driven by Water heaters in terms of revenue while coffee machines and microwaves contribute less. To maximise revenue from this category,strategies to increase sales basket value can be devised during the high demand periods. 

Cameras and camcorders is the third highest revenue generating category with a mid range AOV, demonstrating that again this is a high priced niche category which has less total orders but has high per order purchase. This category is driven by Camcorders which generate the highest revenue while digital cameras contribute the least. Both sub categories have comparable units sold but Camcorders have a high AOV in comparison to digital cameras. The difference in performance is due to price points and not a lot due to demand. 


**Top Order Volume generating products-**

Computers is not only the highest revenue generating but highest selling category in terms of order volume with a total of 15K units sold with desktops being the highest selling sub category. 

Cell phones are the second highest contributor to order volume(**2,715 orders**) after computers and drive a good share of revenue. Revenue from this category does depend on order volume since per purchase amount spent is less. This category is led by Touch Screen Phones and Smart phones & PDAs which generate comparable revenue. 

Music Movies and Audio Books is the third highest contributor to order volume(**2,609 orders**) but generates low revenue indicating that this is again a volume driven category with low price points. This has only one subcategory of Movie DVDs with two brands offering products. Since this category does have demand indicated by the order volume, a new brand and product variations can be introduced with different pricing and the performance can then be monitored. 


### Performance across stores in the United States

There are a total of **20 stores** in the United States spread across different regions. The top 3 stores in terms of revenue are StoreKey 50,54,55.

Analysing further to see if store performance impacts revenue across categories shows that **store performance does have an impact in sales across categories**.

Monthly analysis across revenue, order volume, month-on-month growth, and AOV reveals that some stores experience recurring **slack months with zero sales**, while others continue to generate revenue during the same periods. This pattern is observed across all categories. Encouragingly, the frequency of such slack months has declined over time, indicating improved store–category coverage and greater demand consistency compared to earlier years.

Apart from the year end Q4 spike, there are **seasonal spikes across the months of April to June** with spikes in revenue being **prominent in May** across majority stores for all product categories through all  years till 2019. These spikes could indicate increased demand in the summer months while overall sales in Q1 and Q2 are slow. 

Another pattern found across some outlets is that certain stores **are not showing month on month revenue growth** in  **Q4** which is **alarming** because Q4 is the main heavy demand season. This pattern is again seen across categories and could have an impact specifically in case of high revenue generating categories like computers. 


### Customer Profile Analysis

In the United States there are ~ **7K customers** generating a revenue of 23M. Across age groups, the numbers are comparable except for the **disparity in 18-24** where customer count is extremely low in comparison to other age brackets. 

This is directly related to the revenue generated through each category, as **other categories have a higher revenue generation** in comparison to 18-24. 

With a total population of the United States being ~ 331M in 2020, this market has huge potential and we need strategies to increase the customer base. 

On analysing repeat purchase behavior, while repeat purchasing has increased steadily over time, the low absolute values indicate that **customer retention remains weak** overall and we need stratergies to increase retention which have the potential to improve revenue outcomes. 

Across all these age groups three product categories have shown a constant increase in the revenue year on year - **Audio, Cell phones and Computers**. Efforts should be put into devising strategies to maximise outputs from here since they cater to all age groups. 


## Recommendations

1. Analyse underperforming stores in Q4 and replicate best practices from high-growth locations to maximise performance during peak demand.

2. Introduce loyalty and rewards programs to improve customer retention, increase repeat purchases, and reduce recurring monthly revenue slumps, while enabling more personalised, data-driven customer engagement.

3. Strategic partnerships with third-party distributors could broaden distribution channels and support customer base expansion in the U.S., which currently stands at approximately 7K customers.

4. Strategy development for the Audio, Computers, and Cell Phones categories is likely to be more straightforward, given their consistent year-over-year revenue growth across age groups.
   


## Questions to Stakeholders, Assumptions & Caveats


### Questions to Stakeholders before Progressing in the Project

1. Are there any discount strategies or promotional campaigns applied historically?
   
*The dataset only includes the product unit price, not actual sale prices or discounts.*

2. What defines a successful order — revenue volume, frequency, or customer retention?
   
*This would help refine KPIs and prioritize analysis dimensions accordingly.*

3. Do we want to track repeat customer behavior and long-term value?
   
*This may require additional data on customer retention, satisfaction, or loyalty programs.*



### Assumptions

1. All sales are assumed to be at full unit price.
   
Since no discount, promotional, or negotiated prices are provided, revenue is calculated as:

Revenue = Quantity × Unit Price

2. Product cost and unit price are fixed over time.
   
There's no time-based fluctuation captured in product pricing.

3.  StoreKey 46,52,58 and 60 have shown no sales in this four year period and thus have not been taken into considerating.

### Caveats

1. Revenue is estimated using full Unit Prices without considering discounts, returns, or promotional pricing.

2. The analysis does not factor in currency exchange rate volatility over time — all revenue figures are calculated in USD using the provided static rates.

3. Pricing remains constant for the 4 year period as there's no data given for price volitality. 

## Next Steps

1. Price Elasticity Analysis:
   
Extend the analysis by introducing simulated price increases and decreases to evaluate demand sensitivity, as current cost data is static.

3. Market Basket Analysis:
   
Analyse co-purchasing patterns to identify products that are frequently bought together and assess potential bundling opportunities.










