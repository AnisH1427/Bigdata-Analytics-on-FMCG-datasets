# Bigdata Analytics on FMCG datasets.
This project is utilizes Python, Sparks, scikit learn ,plotly, matplotlib,numpy, pandas, scikit learn
The research project was done in module 6CS012 Bigdata.

### Background 
Big data analytics is the technique of analyzing large and
complex data sets to find patterns and other information that
is important to understand. It consists of using the complex
algorithms such as statistical analysis, machine learning, and
data mining to analyze the data that is in a high volume, high
velocity, and high variety.
Company uses big data analytics in the 21st Century to increase their competitive advantage, improve decision making,
and foster innovation. Businesses can use huge amounts of
structured and unstructured data from social media, sensors,
transaction history, and web traffic to obtain information about
their customers, improve operational efficiency, as well as
create a new generation of products and services to meet the
market’s needs. In our case we have Fast Moving Consumer
Goods (FMCG) for analyzing. We are going to begin through
understanding its datasets and business domain from this
section.

### Data Description
1) invoice: This column contains a unique identifier assigned to each sales transaction for tracking and referencing specific purchases made by customers.
2) orderid: Similar to Invoice, Order ID also serves as a
unique identification number for each order placed by
customers. The only difference is invoice is generated
after the product is received but the Order ID is generated when customers demand the product. At the end,
these both fields are two wheels of the same vehicle.
3) category: The Category column is a broader representation for categorizing products based on their similarities
and the purpose it was intended to use. For example,
the product may be categorized as Food, Juice, Energy,
Beer, Personal Care, cosmetics, and so on.
4) subcategory: Within each Category, products are further
classified into Subcategories based on more specific
attributes inside the same categories. For instance, Subcategories like Snacks, Grains, Protein, nuts, Vegetable,
Chocolates can be included under the Food category.
5) subgroup: Subgroup is an additional level of classification under Subcategory. It facilitates detailed analysis
and reporting by organizing products into more granular
groups. For example, within Snacks Subcategory, Potato
Chips, Popcorn, Noodles, Daalmoth can be included.
6) groupname: Group Name column provides a broader
classification that encompasses Categories, Subcategories, and Subgroups. It categorizes products at a
higher level of abstraction, rather than providing detailed
categorizations.
7) tax application: This column indicates how taxes are
applied to products or transactions. It helps in understanding the tax treatment of products and ensures
compliance with tax regulations.
8) stock method: The Stock Method column in the dataset
indicates the method used for managing inventory. This
column contains two categorical options: FIFO and
Average. These represent different approaches while
valuing inventory and determining the cost of goods
sold (COGS). FIFO stands for First In, First Out, where
the oldest inventory items are assumed to be sold or
used first, followed by newer items. The Average method
typically referred to as the Weighted Average method,
calculates the average cost of all units in inventory,
regardless of when they were purchased.
9) product addedon: This column contains the date when
a product was added to the dataset. It provides metadata
about the timing of data entry and can be useful in data
governance and quality control.
10) productupdatedon: Similar to Product Added On, this
column indicates the date when information about a
product was last modified in the datasets. It can also be
helpful in tracking changes of product data over time.
11) typeofproduct: Unfortunately, in our datasets, the types
of products column consist only of a single type, that is
the product itself.
12) product: This column contains the name, brand and
description of the product being sold. It represents what
type of product is to be served and helps in understanding the specific items in each sales transaction. The same
product can also vary here, for example large size of
toothpaste and small size of toothpaste of same brand
can be considered differently.
13) productAlias: It is a primary identifier of the products.
It helps in accommodating variations in product details
and is represented by the brand name of a Product.
14) salesId: It is a unique ID assigned to each sales transaction to track individual sales records and facilitates
analysis of sales performance metrics like Selling price,
Maximum retailed price, and quantity sold.
15) productId: It is a unique ID for each product in the
dataset. It serves as a reference key for linking sales
transactions to specific products and helps in understanding product-level metrics.
16) Sales Price: It is the price at which the product was
sold in the sales transaction. This field can help to get
insights into pricing strategies, revenue generation, and
customer purchasing behavior.
17) mrp: MRP (Maximum Retail Price) is the highest price
at which the product can legally be sold to consumers.
It can be useful in understanding pricing dynamics and
ensures compliance with regulatory requirements.
18) soldqty: Sold quantities indicates the quantity of the
product that was sold in sales transaction. It may help in
analyzing sales volume, demand patterns, and inventory
management metrics.
19) orderdate: This field represents the date when the order
was placed by the customer. It provides temporal information for analyzing seasonality effects and customer
purchasing behavior over time.
20) invoice date: Invoice date is the date when the invoice
was issued for the sales transaction. It can be useful in
tracking the timing of sales transactions and facilitates
analyzing of revenue and sales performance metrics over
time.

### Business Domain
Having analyzed the data sets we mentioned so far, we can
deduce our business domain as an FMCG sector, which is the
fast-moving consumer goods market. FMCG, for the most part,
implies the products that are in demand rapidly and cheaply
and this includes products such as food, beverages, household
goods, and personal care products. This area features a large
turnover, busy shopping days, or high frequency buying, and
there are multiple contenders for the top position. A breif topic
of the descipline of the businesses determined by the datasets
as follows:
• Product Portfolio: Here, it should be noted that the
dataset had data about various FMCG products including
their categories, subcategories, with each of the items
being provided a detailed description. These goods are
a representative reflection of the assortment of consumer
goods that the retail store has to offer.
• Sales and Distribution: The dataset consists of the items
comprised of sales related data like invoices, order IDs,
sale cost price, quantity sold and the date of transactions.
It is clear, however, that the operation of the business
is carried out by selling FMCG goods to customers by
means of different distribution channels.
• Inventory Management: The appearance of “stock
method” relays that the business carries out its inventory
management with different methods e. g. FIFO (First In,
First Out) and weighted average. Stock availability, minimum out of stock, and optimal storage space utilization
are the most vital points inventory management should
imbibe in FMCG industry.
• Taxation: The info for example tax application shows that
the charge is incorporated with sales transactions. It is
crucial to know the tax regime affecting FMCG businesses, so that they can report financial data accurately
and fulfill the regulatory requirements
• Competitive Landscape: In the personal product marketplace there are numerous different brands competing for
shares. Business, therefore, has to translate its product
preferences and lay the foundation for its future marketing activities. Thus, it should differentiate its products
according to their importance in view of the emerging
consumer preferences to stay ahead of the game or remain
competitive in the market.


### **Lifecycle of Project**
![img.png](assets/img.png)

### **Some insights**
![img_2.png](assets/img_2.png)
![img_3.png](assets/img_3.png)
![img_4.png](assets/img_4.png)
![img_5.png](assets/img_5.png)
The graph shows the Total Sales Over Time from 2021-01
to 2024-01. The y-axis represents the total sales, with a range
from 0 to 160. whearas, x-axis contains the date with the time
intervals. We can gain the following understanding from the
above graphs.
• The highest peak in total sales occurs around 2022-01
where it reaches almost 140.
• The lowest point in total sales occurs at 2021-05, dropping total sales to 20.
• The overall trend shows an increase in sales from 2022
to 2024, with some variations and fluctuation on the way.

![img_6.png](assets/img_6.png)
![img_7.png](assets/img_7.png)
![img_8.png](assets/img_8.png)
![img_11.png](assets/img_11.png)
The chart gives the detail of ”Top 3 Most Used Product
Units”, which comprise of different measurement units.

• 0 - Here we find the products that are not measured in
weight, and they make up 34.6% of the total.

• 24.4% for ’G’ and 19.9% ’GM’ both are expressed in
grams and combinely we can called that 47.% of total
products are represented in grams.

• ’ML’ - This category includes milliliters and covers
11.9% of the total products units.

• ’KG’ - This corresponds to kilograms and contains the
7.1% of the total product units.

• ’L’ - It is liters and is assigned the number 2.1% of the
total unit.

### ElasticSearch Dashboard
![img_9.png](assets/img_9.png)
![img_10.png](assets/img_10.png)
![img_12.png](assets/img_12.png)
![img_13.png](assets/img_13.png)
![img_14.png](assets/img_14.png)

###  No of Components for PCA
![img_15.png](assets/img_15.png)
![img_16.png](assets/img_16.png)

## Clustering
**Algorithm Used: Kmeans++**
### **Finding Optimal K**
![img_17.png](assets/img_17.png)
![img_18.png](assets/img_18.png)
![img_19.png](assets/img_19.png)

**After Analyzing Elbow and Silhouette Score, we decided to go with 5 cluster by considering time and computation**

Interpreting our clusters
![img_20.png](assets/img_20.png)
![img_21.png](assets/img_21.png)

### Metrics 
![img_22.png](assets/img_22.png)

