# Global-Electronics-Retail-Sales-2016-2021

## Background & Overview

**Nexora Electronics** is a fictitious global electronics retailer with operations spanning North America, Europe, and Australia. The company offers a diverse range of consumer electronics spread across 8 categories- Computers, Cell phones, TV and Video, Home Appliances, Music Movies and Audio Books, Audio, Cameras and camcorders, Games and Toys. Nexora’s omnichannel strategy allows it to sell products both through its e-commerce platforms and physical retail stores which are present in 8 countries- United States, United Kingdom, Germany, Australia, Canada, France, Italy and Netherlands.

This project is built on six years of transaction-level data (from 2016 to 2021) includes multiple interconnected datasets, covering:

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

The business generated a total revenue of $55M through 26K orders with a profit of ~ $27M in the years 2016 to 2020.

R**evenue and order volume showed a parallel upward trend till 2019 and dropped significantly in 2020 due to the pandemic. Over the years a quarterly trend emerged, where revenue and growth showed a decline from Q1 to Q2 and then an increase from Q3 to Q4. This pattern can be explained by the end of year festive surges.** 

The **major drivers** of the seasonality trend were- **computers, cameras and camcorders, cell phones and TV and Video**. 

Overall, computers were the major contributor in revenue and order volume. Games and Toys were the least contributors to revenue while TV and Video category drove the least orders. Profit margins were comparable across product categories. 

Regionally, the **United States** contributed to nearly half of the total revenue while countries like France earned the lowest revenue but the AOV was comparable across the countries which indicates that differences in order volume led to the differences in performance. 

Since the United States drove a revenue of ~23M which is almost half of the total revenue, the focus is on this market to identify levers of growth and areas of improvement. 



<img width="575" alt="image" src="https://github.com/user-attachments/assets/0f498306-4ef2-4c83-80c0-c06569037237" />





## Insights Deep Dive

### Product Performance In United States


Similar to the overall product trend, computers are the most important category in the United States driving a  total revenue of $ 8,015K  with ~5K orders.
Within computers the desktop sub category drove revenue generating a total of $4M while the accessory parts like printers, scanners and Fax generated the least revenue of $316K. Since this is a high performing category driven by desktops, during the peaks in Q4 high selling SKUs can be meaningfully bundled with accessory parts to increase basket value. 

Home Appliances is the second highest revenue generating with the highest AOV, which explains that this is a high priced category where users don’t buy frequently but spend heavy amounts per order. This category is driven by Water heaters in terms of revenue while coffee machines and microwaves contribute less. To maximise revenue from this category,strategies to increase sales basket value can be devised during the high demand periods. 

Cell phones are the second highest contributor to order counts after computers and drive a good share of revenue. Revenue from this category does depend on order volume since per purchase amount spent is less. This category is led by Touch Screen Phones and Smart phones & PDAs which generate comparable revenue. 


### Performance across stores in the United States

There are a total of **24 stores** in the United States spread across different regions. The top 3 stores in terms of revenue are StoreKey 50,54,55.

Further analysis of store performance revealed that stores with StoreKey **46,52,58 and 60** have shown **no sales in this four year** period and need to be looked into.

Store with StoreKey **63** has had **no sales through 2020** across all product categories despite sales being generated from all other stores during this period and thus needs to be further investigated.  

Analysing further to see if store performance impacts revenue across categories shows that **store performance does have an impact in sales across categories**.

Monthly analysis across years in terms of revenue, month on month revenue growth and order count and AOV reveal that across  some stores there are certain **slack months** in the year where there is **no sale** while other stores show revenue growth in those months, a pattern seen across all categories. 

Apart from the year end Q4 spike, there are **seasonal spikes across the months of April to June** with spikes in revenue being **prominent in May** across majority stores for all product categories through all  years till 2019. These spikes could indicate increased demand in the summer months while overall sales in Q1 and Q2 are slow. 

Another pattern found across some outlets is that certain stores **are not showing month on month revenue growth** from October to December in **Q4** which is **alarming** because Q4 is the main heavy demand season. This pattern is again seen across categories and could have an impact specifically in case of high revenue generating categories like computers. 


### Customer Profile Analysis

In the United States there are ~ **7K customers** generating a revenue of 23M. Across age groups, the numbers are comparable except for the **disparity in 18-24** where customer count is extremely low in comparison to other age brackets. 

This is directly related to the revenue generated through each category, as **other categories have a higher revenue generation** in comparison to 18-24. 

With a total population of the United States being ~ 331M in 2020, this market has huge potential and we need strategies to increase the customer base. 

Across all these age groups three product categories have shown a constant increase in the revenue year on year - **Audio, Cell phones and Computers**. Efforts should be put into devising strategies to maximise outputs from here since they cater to all age groups. 



## Questions to Stakeholders, Assumptions & Caveats


### Questions to Stakeholders before Progressing in the Project

1. Are there any discount strategies or promotional campaigns applied historically?
   
*The dataset only includes the product unit price, not actual sale prices or discounts.*

2. What defines a successful order — revenue volume, frequency, or customer retention?
   
*This would help refine KPIs and prioritize analysis dimensions accordingly.*

3. Do we want to track repeat customer behavior and long-term value?
   
*This may require additional data on customer retention, satisfaction, or loyalty programs.*

## Recommendations

1. For the main driver category- computers, certain stores show low or moderate growth rates during October to December across 2016-2019. This is alarming because these are the peak selling periods, thus we should be further checking in store performances and possibly replicating strategies followed by stores showing high growth rates during this period.
   
 2. Across categories throughout the years there are certain slack months where there is no sale across some stores.Investigation needs to be done to check if this slack is due to lack of demand in that region where the store is or due to some other reason.
     
3. For all categories there are seasonal spikes specially in the months of April to June with spikes being prominent in May across majority stores and across all years till 2019. This needs to be further seen as to what’s driving these spikes-could be attributed to seasonal summer sales. We could target these periods to maximise sales with promotional offers.

4. The total customer base is ~7K in the United States.Disparity exists across age groups where 18-24 is under represented. With a total population of the US being 331M, we need to devise strategies to increase the customer base through more stores? certain promotions like discounting?
   
5. Audio, computers and cell phones see revenue growth year on year across all age groups, thus expending all efforts on these categories would lead to overall revenue growth. Product teams can further monitor which sub categories and brands show more growth across different age groups?? New products can be added?? Schemes during holiday seasons to increase revenue here?


### Assumptions

1. All sales are assumed to be at full unit price.
   
Since no discount, promotional, or negotiated prices are provided, revenue is calculated as:

Revenue = Quantity × Unit Price

2. Product cost and unit price are fixed over time.
   
There's no time-based fluctuation captured in product pricing.


### Caveats

1. Revenue is estimated using full Unit Prices without considering discounts, returns, or promotional pricing.

2. The analysis does not factor in currency exchange rate volatility over time — all revenue figures are calculated in USD using the provided static rates.












