# Python_RFM_Analysis: Customer segmentation
Utilize the RFM model to segment customers and recommend suitable marketing campaigns.
## I. Introduction
### 1. Project's context: 
- SuperStore is a global retail company with a large customer base. On the occasion of Christmas and New Year, the Marketing department wants to run marketing campaigns to express gratitude to customers who have supported the company over time and to tap into potential customers to turn them into loyal ones. 
- However, the Marketing department has not yet segmented customers for this year due to the large dataset, which cannot be processed manually as in previous years. Therefore, they are seeking support from the Data Analysis department to deploy a customer segmentation task to classify each customer segment and tailor marketing programs accordingly.
- The Marketing Director has also proposed using the RFM model. However, in the past, when the company was smaller, the team could calculate and classify using Excel. With the current large volume of data, they hope the Data department can build a deployment pipeline for segmentation evaluation through Python programming.
### 2. Business question
- SuperStore is a global retail company. The Marketing Department wants to run marketing campaigns during the Christmas and New Year holidays to thank customers for their past support of the company. In addition, potential customers can be upgraded to become loyal customers.
- The Marketing Director also proposed a plan to use the RFM model in Python to segment customers and then launch appropriate marketing campaigns. Analyze the current situation of the company and give suggestions to the Marketing team
- With the retail model of Superstore company, which indicator should be most focused on in the 3 indicators R, F, and M?
### 3. Dataset
This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

- **InvoiceNo**: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'C', it indicates a cancellation.
- **StockCode**: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
- **Description**: Product (item) name. Nominal.
- **Quantity**: The quantities of each product (item) per transaction. Numeric.
- **InvoiceDate**: Invoice Date and time. Numeric, the day and time when each transaction was generated.
- **UnitPrice**: Unit price. Numeric, Product price per unit in sterling.
- **CustomerID**: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
- **Country**: Country name. Nominal, the name of the country where each customer resides.
### Segmentation
<img width="677" alt="Screenshot_1" src="https://github.com/NuongLe123/RFM_analysis/assets/168357450/75ba6d99-afc1-4977-9ded-cbd752765692">

### 4. RFM model
- RFM (Recency, Frequency, Monetary) analysis is a method used for analyzing customer value. Specifically, it is a marketing model using customer segmentation based on their transaction history.
- This model could be very useful, especially for small and medium-sized enterprises (SMEs) with limited marketing resources, helping them focus on the potentially right customer segments to increase ROI, reduce churn, reduce cost, improve customer relationship, and a lot more.
- RFM stands for the three dimensions:
Recency – How recently did the customer purchase?
Frequency – How often do they purchase?
Monetary Value – How much do they spend?

## II. Insights & Recommendations:
<img width="1027" alt="Screenshot_4" src="https://github.com/NuongLe123/RFM_analysis/assets/168357450/dd3b4a70-ccc1-4d0b-ab0f-e6bf81529511">
<img width="1023" alt="Screenshot_5" src="https://github.com/NuongLe123/RFM_analysis/assets/168357450/c4f3731b-cb85-453b-8cb2-264488b18653">
<img width="1053" alt="Screenshot_6" src="https://github.com/NuongLe123/RFM_analysis/assets/168357450/7272e13d-4c9d-45ff-940f-d04bd2c3c5fb">

- **Recency distribution** is right-skewed, showing that the majority of customers made a purchase in the recent past. It has a long tail containing single customers who made their order long time ago. Similar pattern also appears on **Frequency and Monetary** distribution plots. The plots show that most customers has low frequency (small number of orders, around 10 per customer) and spend little amount of money in each transaction.
- Although the information is quite general (since we're using distribution plot and there might be other factors affecting the results), we've gained some insights of experiences of our customers, and find out the reasons why the RFM indicators are so low.


<img width="980" alt="Screenshot_7" src="https://github.com/NuongLe123/RFM_analysis/assets/168357450/6363fa0d-9e65-4470-88da-20e46e3b423c">

- As can be seen from the 'RFM Segments of Customer Count', it is obvious that the **'champions' group** not only has the highest number of customer (about 19%) but also make largest contribution to company’s sales.
- It should be considered that group of **'hibernating'** is so big (about 15%). It is suggested that offering other relevant products and special discounts to this customer segmentation. Besides, the company should focus on the group **'at risk'** to increase customer retention.
- **'Loyal customers' and 'potential loyalists'** constitute about 11% and 10% of the total customers.


<img width="899" alt="Screenshot_3" src="https://github.com/NuongLe123/RFM_analysis/assets/168357450/08bf1484-94c1-4571-b2be-2a20e1902c06">

- **The champions and loyal segmentation** contribute the majority of sales to the company (totally approximately 75%). This means that they are quite satisfied with products of company. Therefore, the company can reward them and give them early access of new products. Besides, it is recommended that we should upsell higher value products and asking their reviews so that they can be our loyal customers in the future. 
- **At risk and loyal group** make contributions of 8% and 11% of total sales respectively. This type of group is known as spending big money and purchasing often long time ago (recency problems). Therefore, we need to send them personalized emails to reconnect, offer renewals and offer special deals with the hope of bringing them back. 
- Despite the large number of customers, **potential loyalist** only spent a little amount of money (about 2.5% in total sales). For this group, it is necessary to offer membership or loyalty program and recommend other products.
- The last two types is **hibernating and lost customers**. For hibernating, the company can reactivate them by offering other relevant products as well as special discounts and recreating brand value. Try all the best to prevent this group from converting into lost customers group. As for lost customers, we should ignore them, since their small contribution to sales (1%).



