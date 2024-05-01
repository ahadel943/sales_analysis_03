# Sales Analysis

# Introduction

In the ever-evolving landscape of commerce, data serves as the compass guiding organizations towards informed decision-making and strategic growth. Within this dynamic environment, our Sales Data Analysis Project stands as a beacon of insight, illuminating the pathways to enhanced performance, optimized strategies, and sustainable success.

## Tools used
1) Microsoft Excel 2016.
2) Power Quer for data extraction, cleaning and prepration.
3) Pivot Tables for analysis and insights.

## Business Questions and Tasks

1) **Time Series Analysis:**
    * **Trend Analysis:** Examine the trend of sales over the four-month period, looking at changes in sales amount over time.
    * **Seasonality Analysis:** Look for patterns within the four-month period, such as increased sales during specific weeks or on certain days of the week.

2) **Product Analysis:**
    * **Product Performance:** Compare sales across different product categories and types during the four-month period.

3) **Geographical Analysis:**
    * **Region Performance:** Compare sales performance across different regions to identify strengths and weaknesses.

4) **Customer Segment Analysis:**
    * **Customer Segment Performance:** Analyze sales performance across different customer segments to understand which groups are driving the most revenue.

5) **Salesperson Analysis:**
    * **Salesperson Performance:** Compare the performance of different salespeople during the four-month period.

## Data cleaning and preparatrion

After cleaning, preparing and understanding the data found the following notes

1) The dataset includes 40 records.
2) No missing values or outliers were found.
3) New features were generated **Year, Month, Month ID, Weekday and Weekday ID**.
4) The dataset contains 12 features.

## Data Features								

| Column | Count | Type |
| ------ | ----- | ---- |
| Date | 40 | DATE |
| Product Category | 40 | TEXT |
| Region | 40 | TEXT |
| Salesperson | 40 | TEXT |
| Customer Segment | 40 | TEXT |
| Product Type | 40 | NUMBER |
| Sales Amount | 40 | CURRENCY |
| Year | 40 | NUMBER |
| Month | 40 | TEXT |
| Weekday | 40 | TEXT |
| Month ID | 40 | NUMBER |
| Weekday ID | 40 | NUMBER |

## Conclusions

1) key performance indicators (KPIs):
    * Orders Count: 40 orders
    * Total Sales Amount: $203,600
    * Average Order Value (AOV): $5,090
    * Minimaum Order value: $3,500
    * Maximum Order VAlue: $6,600
    * Sales Standard Deviation: $758 (**January $772**, **February $729**, **March $721** and **April $724**).

2) Based on our time series analysis the following was found:
    ![total_sales_amount_by_month](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/1.total_sales_amount_by_month.jpg)
    * The sales amount has been increasing steadily over the four-month period, from **$47,300** in **January** to **$54,400** in **April**. This indicates positive sales growth over time.
    * **January: $47,300**
    * **February: $49,600**
    * **March: $52,300**
    * **April: $54,400**
    * Month-over-Month (MoM) Growth Rate:
    * **January** to **February**: **4.86%**
    * **February** to **March**: **5.44%**
    * **March** to **April**: **4.02%**
    * While the overall trend is positive, there are fluctuations in the growth rates from month to month. Understanding these fluctuations can help identify seasonal patterns or the impact of specific events or promotions on sales performance.
    ![total_sales_amount_by_weekday](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/2.total_sales_amount_by_weekday.jpg)
    * In the month of **January**:
      * Highest Sales: **Tuesday** (**$9,300**)
      * Lowest Sales: **Thursday** (**$3,800**)
    * Sales tend to peak mid-week, with **Tuesday** recording the highest sales.
    * Sales are relatively lower towards the end of the week, particularly on **Thursday** and **Friday**.
    * In the month of **February**:
      * Highest Sales: **Friday** (**$9,700**)
      * Lowest Sales: **Sunday** (**$4,200**)
    * Sales peak towards the end of the week, with **Friday** recording the highest sales.
    * **Sundays** have the lowest sales compared to other days of the week.
    * In the month of **March**:
      * Highest Sales: **Friday** and **Thursday** (**$10,200** and **$9,900** respectively)
      * Lowest Sales: **Sunday** and **Saturday** (**$4,500** and **$6,000** respectively)
    * **Friday** and **Thursday** consistently record the highest sales throughout the week.
    * Sales are relatively lower on weekends, especially on **Sundays**.
    * In the month of **April**:
      * Highest Sales: **Monday** (**$10,600**)
      * Lowest Sales: **Wednesday** (**$4,700**)
    * **Monday** records the highest sales in **April**, deviating from the trends observed in previous months.
    * **Wednesday** has the lowest sales compared to other days of the week.
    * There are fluctuations in sales amounts across different days of the week, with certain days consistently recording higher sales than others.
    * **Tuesdays**, **Wednesdays**, and **Thursdays** often see higher sales compared to **Mondays** and **Fridays**, suggesting that mid-week days are more favorable for sales.
    * **Saturdays** generally have **moderate** sales, while **Sundays** consistently have **lower** sales across all months.
    * **While there are some consistent patterns, there are also variations in sales distribution across months, indicating that external factors or seasonal influences may affect purchasing behavior**.
    ![seasonality_Index_(S.I.)_by_weekday](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/12.seasonality_Index_(S.I.)_by_weekday.jpg)
    * **Friday** has the highest seasonality index of **1.08**, indicating that sales on **Fridays** are typically **8%** higher than the overall average sales.
    * **Monday** has a seasonality index of **1.02**, suggesting that sales on **Mondays** are slightly above the overall average by **2%**.
    * **Saturday** and **Sunday** both have a seasonality index of **0.97**, indicating that sales on weekends are slightly below the overall average by **3%**.
    * **Thursday** and **Tuesday** also have a seasonality index of **0.97**, suggesting that sales on these weekdays are slightly below the overall average by **3%**.
    * **Wednesday** has a seasonality index of **1.01**, implying that sales on **Wednesdays** are slightly above the overall average by **1%**.
    
3) Based on our product category performance analysis we found the following:
    ![total_sales_amount_by_product_category](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/3.total_sales_amount_by_product_category.jpg)
    * The **Electronics** category generated the highest income totaling **$125,900** which represents a **61.84%** of the total sales amount.
    * The **Clothing** comes in next with a total of **$77,700** which is **38.16%** of the total sales amount.
    * By breaking down the sales amount by month both categories maintaining nearly the exact same perforrmance the **Electronics** (**61.58%** to **62.37%**) while the **Clothing** (**37.63%** to **38.42%**).
    ![total_order_count_by_product_category](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/4.total_order_count_by_product_category.jpg)
    * Following the same sales pattern both of the categories tend to nearly maintain the same performace in orders count.
    * The **Electronics** generated an order count of **24** orders which is **60%** of the total orders count while Clothing generated a total of **16** orders which is **40%** of the total orders count.

4) The following insights were found in our regional sales analysis:
    ![total_sales_amount_by_region](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/5.total_sales_amount_by_region.jpg)
    * The **North** region leads in sales amount generation with a total of **$92,300** followed by the **West** region totaling **$58,800** and finally the **South** region with a total of **$52,500**.
    * A notable pattern in our regional data the higher the sales generated the higher the average order value, **North** has the highest AOV (**$5,769**) followed by **West** with an AOV of (**$4,900**) and finally **South** with an AOV of (**$4,375**).
    ![total_orders_count_by_region](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/6.total_orders_count_by_region.jpg)
    * The same sales amount and AOV pattern has repeated in the order count distribution with one difference which is the **South** and **West** has the same orders count **12** orders and yet the **West** region generated more sales than **South** the reason for that might be the higher AOV.
    * The **North** region also leads the orders count generated with a total of **16** orders which is **40%** of the total orders amount.

5) Based on the customer segment analysis the following insights were found:
    ![total_order_count_by_customer_segment](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/7.total_order_count_by_customer_segment.jpg)
    * In terms of oders coount both customer segment generated (**Retail** and **Wholesale**) tha same count **20** orders.
    * By breaking down the orders count by month each segment followed the same pattern, **5** orders per month
    ![total_sales_amount_by_customer_segment](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/8.total_sales_amount_by_customer_segment.jpg)
    * Based on our data, **Retail** generated the highest sales amount with a total of **$103,800** which is **50.98%** while **Wholesale** generated **$99,800** in total which represents **49.02%** of the sales totals.
    * Despite of the same orders count for both segment the **Retail** segment generated more sales and it has a higher **AOV** (**$5,190**) while the **AOV** of **Wholesale** segment is (**$4,990**).
    * Except for the month of **February**, **Retail** tends to geneate more sales than **Wholesale**
      * In **January**:
        Retail: **$24,000**
        Wholesale: **$23,300**
      * In February:
        Retail: **$24,200**
        Wholesale: **$25,400**
      * In March:  
        Retail: **$27,900**
        Wholesale: **$24,400**
      * In April:
        Retail: **$27,700**
         Wholesale: **$26,700** 

6) Based on the analysis conducted on our salespersons performance the following insights were found:
    ![total_sales_amount_by_salesperson](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/9.total_sales_amount_by_salesperson.jpg)
    * A notable variation in sales performance with sales amounts ranging from $**17,200** to **$46,700**
    * **John**, **Lisa** and **James** are the top performers with totals of **$46,700**, *$42,700* and **$42,700** respectivly.
    * **John**, **Lisa** and **James** tend to stand out as the top performers across the entire period.
    * **David** and **Emily** fall into the middle range of sales amount, with sales amounts between **$21,000** and **$33,300**.
    * **Michael** has the lowest sales amount among the salespersons with the total of **$17,200**, indicating that there may be areas for improvement in his sales approach or strategies.
    * **Lisa** and **James** both have generated the same sales amount of **$42,700**, This suggests that they may have similar sales strategies or are working with similar client bases.
    ![average_order_value_by_salesperson](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/10.average_order_value_by_salesperson.jpg)
    * As expected there is a notable variation in the salesperson **AOV** ranging from **$4,163** to **$5,838**.
    * John, Lisa and James have the highest AOV $5,838, $5,338 and $5,338.
    * **Michael** has the lowest AOV of **$4,300**
    * **James** and **Lisa** both have the same AOV of **$5,338**.
    ![total_orders_count_by_salesperson](https://github.com/ahadel943/sales_analysis_03/blob/main/charts/11.total_orders_count_by_salesperson.jpg)
    * Another notable variation in our order count generated by salespersons ranging from **4** to **8** orders.
    * **James**, **Lisa**, **John** and **Emily** have the highest order count, **8** orders each.
    * **Michael** and **David** have the lowest order count, with **4** orders each.
    
## Recommendations:

1) Considering that the sales standard deviation for each month (ranging from $721 to $772) are relatively consistent, indicating a similar level of variability in sales amounts across all four months due to such performance the following is recommended:
    * **Optimization of Resources:** understanding the variability in sales amounts can help in optimizing resource allocation and inventory management. By anticipating sales fluctuations, we can ensure that we have the right level of inventory on hand to meet customer demand without overstocking or understocking.

    * **Risk Management:** a consistent level of sales variability can also aid in risk management by allowing we to identify and mitigate potential risks associated with sales fluctuations. By understanding the range of variability, we can implement strategies to minimize the impact of unexpected changes in sales performance.

    * **Stability in Sales Patterns:** the consistent standard deviation values suggest that there are stable sales patterns within each month. This stability can be advantageous for forecasting and planning purposes, as it indicates a predictable level of variability in sales performance.

2) Based on the insights found from the time series analysis we recommend the following:
    * **Optimized Marketing Strategies:**
        * Use the knowledge of peak sales days within each month to schedule targeted marketing campaigns and promotions. For example, focus promotional efforts on Tuesdays and Fridays when sales tend to be higher.
        * Tailor marketing messages and incentives to encourage sales on slower days, such as Sundays, by offering special promotions or discounts.

    * **Seasonal Planning:**
        * Identify seasonal patterns or trends in sales performance and plan accordingly. For instance, if certain months consistently show higher growth rates, allocate more resources and invest in marketing efforts during those periods to capitalize on increased consumer demand.

    * **Product and Pricing Strategies:**
        * Analyze sales data to identify bestselling products and adjust pricing or promotions to maximize revenue. Use insights from peak sales days to introduce new products or offer exclusive deals to drive sales.

    * **Competitive Advantage:**
        * Use our understanding of sales patterns and consumer behavior to differentiate our business from competitors. By optimizing our sales strategies and providing exceptional customer experiences, we can establish a competitive advantage in the market.

3) Based on the findings from the product category analysis we recommend the following:
    * **Focus on High-Performing Categories:** allocate more resources, marketing efforts, and inventory towards the Electronics category, as it generates the highest income and represents a significant portion of total sales. This category seems to be a strong revenue driver for our business.

    * **Identify Growth Opportunities:** while Electronics may be performing well, there could still be opportunities to further grow this category. Explore avenues such as expanding product offerings, introducing new features or upgrades, or targeting specific customer segments to drive additional sales within the Electronics category.

    * **Maintain Consistency:** since both Electronics and Clothing categories maintain nearly the same performance over time, continue to focus on maintaining the consistency of sales within these categories. Monitor sales trends and adjust strategies as needed to sustain the performance levels.

    * **Optimize Marketing and Promotions:** tailor marketing campaigns and promotions to each product category based on their performance and customer preferences. Highlight the unique features and benefits of Electronics products to attract more customers, while also offering compelling deals and promotions to drive sales in the Clothing category.

    * **Customer Segmentation:** analyze customer data to identify the demographics, preferences, and buying behaviors of customers who purchase Electronics and Clothing products. Use this information to target specific customer segments with personalized marketing messages and offers to increase conversion rates and repeat purchases.

4) Based on our insights from the regional sales analysis we recommend the following:
    * **Resource Allocation:** allocate resources, marketing efforts, and inventory based on regional sales performance. Focus more resources on the North region, which generates the highest sales amount and has the highest average order value (AOV). This can help maximize return on investment and drive overall revenue growth.

    * **Targeted Marketing Strategies:** tailor marketing campaigns and promotions to each region based on their sales performance and average order value. Highlight products or offers that resonate with customers in each region to increase sales and customer engagement.

    * **Product and Pricing Optimization:** analyze sales data to identify bestselling products and adjust pricing or promotions to maximize revenue in each region. Consider offering region-specific deals or discounts to capitalize on regional preferences and increase sales.

5) Based on the findings in our customer segment analysis we recommend the following:
    * **Targeted Marketing and Sales Strategies:** tailor marketing messages and sales strategies to each customer segment based on their purchasing behavior and preferences. For example, focus on highlighting different product features or benefits that appeal to Retail customers versus Wholesale customers.

    * **Product Offering and Pricing:** adjust product offerings and pricing strategies to better cater to the needs and budgets of each customer segment. Consider offering bulk discounts or special pricing incentives for Wholesale customers to encourage larger orders, while providing exclusive deals or promotions for Retail customers to drive repeat purchases.

    * **Inventory Management:** optimize inventory levels for each customer segment based on their sales patterns and order volume. Ensure that we have sufficient stock to meet demand from both Retail and Wholesale customers while minimizing excess inventory costs.

    * **Customer Retention and Loyalty Programs:** implement customer retention and loyalty programs tailored to each customer segment to incentivize repeat purchases and increase customer lifetime value. Offer exclusive perks or rewards for loyal Retail customers, such as early access to new products or special discounts, to encourage repeat business.

    * **Market Expansion Opportunities:** Identify opportunities to expand into new markets or customer segments based on the analysis of Retail and Wholesale customer behavior. Use insights from customer segment data to identify untapped markets or niches that align with our business goals and objectives.

6) Based on our salespersons performance analysis we recommend the following:
    * **Performance Recognition and Incentives:** recognize and reward top performers such as John, Lisa, and James for their outstanding sales performance. Implement incentive programs or bonuses to motivate and retain top talent within our sales team.

    * **Training and Development:** provide additional training and support to salespersons with lower sales amounts or AOV, such as Michael. Offer coaching sessions, sales workshops, or mentorship programs to help improve their sales approach and strategies.

    * **Sales Strategy Alignment:** analyze the sales strategies of top performers (e.g., John, Lisa, and James) to identify commonalities or best practices. Align the sales strategies of other salespersons with these successful approaches to improve overall sales performance.

    * **Targeted Marketing and Sales Approaches:** tailor marketing messages and sales approaches to target customer segments that align with the strengths and preferences of each salesperson. Utilize insights from AOV and order count data to identify opportunities for segment-specific strategies and personalized interactions.

    * **Sales Team Collaboration:** encourage collaboration and knowledge sharing among sales team members. Facilitate opportunities for them to learn from each other's experiences, share successful sales strategies, and support each other in achieving common goals.


By leveraging these insights effectively, we can optimize our sales strategies, increase revenue, and improve overall business performance. Continuously monitor our business behavior and adapt our strategies as needed to stay competitive and drive sustainable growth.






