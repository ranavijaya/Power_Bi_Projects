# Introduction
This dashboard offers a comprehensive analysis of product reviews on Amazon, providing valuable insights to assist businesses in enhancing their products, gaining a deeper understanding of customer preferences, and developing effective marketing strategies.
By utilizing this dashboard, businesses can access a wealth of information regarding product reviews on Amazon. Through advanced analytics and data visualization, it presents a detailed examination of customer feedback, allowing companies to uncover hidden patterns, trends, and sentiments.
The insights derived from this dashboard can prove instrumental in product improvement efforts. By identifying recurring issues or areas of improvement mentioned in the reviews, businesses can take targeted actions to enhance their products' features, functionality, or overall quality. This data-driven approach empowers organizations to make informed decisions and prioritize product enhancements based on real customer feedback.

---
## The Structure of Dashboard
The Power BI dashboard consists of four main pages. Each of these components serves a unique purpose and offers different insights into the data.

---
### 1. Summary Page

![Alt Text](./Images/Capture1.png)

The Summary Page provides a comprehensive overview of various metrics and analyses related to customer ratings and product perception. It offers insights into customer preferences, price analysis, and the impact of discounts on ratings. The page features the following components:

- Total Ratings Count and Average Rating: This section showcases the overall number of ratings received and the average rating score. It provides a high-level view of customer satisfaction.

- Rating Bucket Analysis: The page displays the total rating count for different rating buckets, such as 1 to 2, 2 to 3, 3 to 4, and 4 to 5. This analysis helps to understand how customers perceive products based on their ratings.

- Price Vs. Rating Analysis: A scatter chart is used to illustrate the relationship between product prices and ratings. This analysis enables users to identify any correlations or trends between pricing and customer satisfaction.
- Average Ratings by Product Category: This section presents the average ratings across various product categories. It allows users to compare customer satisfaction levels for different types of products. This also gives the sentiment word cloud of the product reviews and the sentiment score of audience.

  ![Alt Text](Images/Capture2.png)
- Discount Vs. Rating Analysis: This analysis focuses on the impact of discounts on customer ratings. It provides insights into how offering discounts affects customer perception and satisfaction.

![Alt text](Images/Capture3.png)

### Other features implemented.

- Slicers -> allow users to filter the data based on specific categories or price ranges. These slicers enable users to customize the displayed information and gain more targeted insights.

- Drill through -This allows users to navigate from a summary report or visual to a more detailed report or page that provides additional context or specific information related to the selected data point on the Discount vs Rating page that routes to product details page. 
![Alt text](Images/Capture4.png)

- Reset button-This is a button that resets all the filters. 
- Page navigation on left.  
- Implemented Dax queries for Rating bucket. 
![Alt text](Images/Capture5.png)

Overall, the Summary Page serves as a valuable tool for businesses to analyze and understand customer ratings, product perception, pricing strategies, and the influence of discounts on customer satisfaction.

---

### 2. Product Table:
![Alt text](Images/Capture6.png)

This page presents a tabular view of products, showcasing important product details for easy reference and analysis. The table includes the following essential information:

-	Product Image: An image representing the product for visual identification.
-	Product Name: The name or title of the product.
-	Product Link: A hyperlink that redirects users to the corresponding product page on the Amazon website for further details or purchasing.
-	Rating: The average rating or customer satisfaction score for the product.
-	Total Ratings Count: The total number of ratings received for the product, indicating its popularity or level of customer feedback.
-	Actual Price: The original or regular price of the product.
-	Discount Price: The discounted price, if applicable, offering potential savings to customers.
-	Discount Percentage: The percentage of discount applied to the product price.

Like the Summary Page, this page also features slicers positioned at the top. These slicers enable users to filter and customize the displayed data based on specific categories or price ranges. Users can interact with the slicers to refine their analysis and focus on products that match their desired criteria.

Overall, this tabular view page provides a convenient overview of products, allowing users to quickly evaluate important details, compare prices, discounts, ratings, and make informed decisions. The slicers enhance the page's usability by offering flexible filtering options tailored to individual preferences.

---
### 3. Decomposition 

![Alt text](Images/Capture7.png)

On the Decomposition Tree page, users can gain valuable insights by drilling down into different dimensions and dissecting the factors that contribute to the average ratings in a comprehensive and interactive manner.

---

### 4. Q&A
![Alt text](Images/Capture8.png)

We can effortlessly pose questions using natural language and receive answers in a visually engaging format.

---
### 5. Product Details / Product Tooltip /Review Pages

#### a. Product details Page
![Alt text](Images/Capture9.png)

The Product Details page provides an array of detailed information, including
-	actual price 
-	discounted price
-	discount percentage
-	total ratings
-   average rating

Displayed through a star rating visual, product image, and description.
To access this page, we can utilize the Drill Through feature at the product level visual from any page, ensuring seamless navigation and a more immersive exploration of the specific product details.
#### b. Tooltip  Page
I have used two tooltips. 
1. Product tooltip- 
Which gives the detail of the product and is hidden. 
![Alt text](Images/Capture10.png)

2. Review tooltip 
It gives popular reviews of the product and gives the sentiment score and is hidden. 
![Alt text](Images/Capture11.png)

---

## 3.Data Transformation/Cleaning:
Data was efficiently cleaned and transformed with the Power Query Editor of Power BI. Few steps are listed below. 

1. Split Column by Delimiter:
![Alt text](Images/Capture12.png)

2. Column Operations:
Converted discounted price and actual price from text to decimal and applied below transformation.
![Alt text](Images/Capture13.png)


3. Data Cleaning :
![Alt text](Images/Capture13_1.png)

The data contains errors shown below for which I replaced them will null values.
![Alt text](Images/Capture13_2.png)

![Alt text](Images/Capture13_3.png)

---

## 4. Conclusions & Recommendations
The dashboard offers comprehensive and detailed analysis through dedicated pages, allowing users to gain both an overview and a granular breakdown of the data. With an intuitive interface, user-friendly filters, and an interactive Q&A feature, the dashboard is designed to be easily accessible and navigable. By providing data-driven insights, the dashboard empowers users to make informed decisions quickly and efficiently, enhancing the decision-making process for businesses.
-	Implementing a feature to send discount coupons directly to customers who provide reviews on your site, incentivizing their engagement.
-	Recognizing and highlighting top agents who consistently solve customer tickets effectively, motivating them to provide excellent service and improve customer satisfaction.
-	Tracking product sales and generating revenue reports to monitor performance, identify top-selling products, and optimize business strategies.
-	Integrating data from external datasets to gain more insights and enhance the system's capabilities.
-	Analyzing overall satisfaction by different age groups to understand customer preferences and tailor marketing strategies accordingly.
-	Analyzing the age groups of review posters to target specific demographics and improve review-centric strategies.
-	Tracking the number of orders placed versus returns to assess customer satisfaction and identify areas for improvement.

By incorporating these features, we can optimize the system, improve customer satisfaction, and make   informed decisions for business growth.

---

# 5. Links
The dashboard link is below
[Amazon Review](https://app.powerbi.com/links/CDUPSGTqv6?ctid=96464a8a-f8ed-40b1-99e2-5f6b50a20250&pbi_source=linkShare&bookmarkGuid=50bc35c6-c46c-42e8-93f3-7985517264c0)
