# Marketing-Retail-Analytics_Capstone_Project

# Business Background

In the recent past, e-commerce companies have emerged and flourished in the industry. They offer the convenience to order from a wide variety of options from the comfort of one’s home. But how do they offer these “wide variety of options or products”? To be able to meet the demands of the customers, any e-commerce company would obviously need to store tons and tons of products in warehouses. Now, some of these warehoused products might be fast-moving products which sell very quickly and some others might be slow-moving. Each of the products being stored incurs a cost to the company in terms of space and maintenance. Since storing these products obviously add to the costs that the company incurs, it is absolutely necessary for the organisations to plan their inventory well.

# Problem Statement 

Now, OList is one such e-commerce company that has faced some losses recently and they want to manage their inventory very well so as to reduce any unnecessary costs that they might be bearing. In this assignment, you have to manage the inventory cost of this e-commerce company OList. You need to identify top products that contribute to the revenue and also use market basket analysis to analyse the purchase behaviour of individual customers to estimate with relative certainty, what items are more likely to be purchased individually or in combination with some other products.
Also, you need to help OList to identify the product categories which they can get rid of without significantly impacting business.

Some other important aspects that you should consider, such as:
  - What should be the ideal category depth?
  - Some product combinations are sold more than others. This needs to be understood using market basket analysis.
  - After having specific categories in hand that will be beneficial to the company, how can you reduce the number of items in a particular category?

After gaining insights from the dataset, you will need to present your solution along with visualisation in the form of a dashboard and supplement it with an executive summary. This will help the team at OList to take the required action based on your recommendations.

# Flow of capstone project:
- 1) Performed Data Cleaning and EDA using python
- 2) Exported the cleaned data into 2 .csv files
     - file1 - Used complete cleaned data for further visualization and dashboard in Tableau.
     - file2 - Transformed data to perform Self Join in Tableau for Market Basket Analysis in Tableau.
- 3) Performed in-depth EDA and extracted insights and presented them in form of dashboard.
- 4) Performed Market Basket Analysis and made dashboard to present the important insights.
- 5) Given Recommendations based on the obtained insights.
- 6) Concluded the effects of recommendations on the business revenue and inventory mix.
 
# Some of the Important insights

- 1) Dashboard 
 
# Recommendations
- We can reduce the category breadth by only focusing on 27 categories which are frequently selling together like toys, bed_bath_table, furniture_decor, computer accessories etc. at the cost of only 3 % revenue hit while reducing the inventory by almost 900 unique products.
- If category depth is high then it can be reduced by targeting 80% or 90% revenue from that category and retaining only the top revenue generating products which can help us achieve the revenue target. 
- Although toys being highest selling as well as revenue generating category, it is the main culprit behind excessive inventory management costs, we can get rid of the products from toys category with only single unit sales and still achieve 75% of the current revenue from toys category and cater to 83% of the customer demand (toys orders) but on the contrary reduce the toys inventory by 
almost 60%.
- Personalized suggestions and recommendations is required to increase the purchase of products in combination with other products or categories.
-  It is recommended to avoid any abrupt changes in the inventory mix, gradual implementation of the above strategies would make sure that the customers also get some time to adapt to the changes.
- If possible, the products which we would discontinue or get rid from our warehouse, should be kept under ‘on demand’ order category so that we can outsource that product and deliver it to customers. This would ensure that we don’t lose the customer to our competitor.


# Conclusion

- Initially, if we focus on only top 27 categories, we can achieve almost 90% revenue while reducing the inventory by approx. 25%. 
- Categories which show comparatively higher confidence (more than 10%) of purchase along with toys are bed_bath_table, construction_tools_lights, construction_tools_garden, fashion_bags_accessories, fashion_shoes.
- While reducing the category depth, it is important to keep an inventory mix of fast moving and slow moving inventory to maintain the revenue as well as inventory management costs.
- Low revenue generating Non-moving inventory could go under ‘on-demand’ order category.

# Data Sources :

1) Here is a snapshot of the data dictionary
  - Orders information like unique order_id, order_item_id, order purchase-approval-delivery timestamp. etc
  - Customer’s information like unique customer_id, zipcode, city and state
  - Payment information like payment_value, payment_type etc.
  - Product dimension and specification information like category, weight, length etc.
  - Customer preference information like number of reviews and number of reviews per month
2) The provided data is captured from the CRM tool used by ‘OList’. (till 17-10-2018 17:30).

# Data Methodology :
- Checked the data for any duplicate, null, insignificant values and Cleaned using python.
- Checked for outliers, as outliers were actual values, the values were kept as it is, instead used median as central measure.
- Merged the datasets for further analysis and performed EDA.
- Created new dataset with only order_id and product_category for Market Basket Analysis.
- Exported the cleaned datasets in Excel format to upload in Tableau.
- Used Tableau for visualization of data and created appropriate calculated fields to get the insights.

