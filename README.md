# Insiders Clustering
![capa linkedin](https://user-images.githubusercontent.com/77075354/156940134-007ec87d-e28f-466e-9096-f71e03f0cbc1.jpeg)

The Insiders Clustering is a company loyalty program that belongs to All In On Place. It is aimed for a small number of clients who have a high sales volume or, for those who buy products of higher value. These clients generate representative values for the billing of the company. They are high valued customers, and this is why they need to be retained.

### Aimed of Project

Identify monthly who are the clients eligible from the program of customer loyalty, as well as, create new marketing strategies for inserting potential customers in the Insiders Clustering group.

### Business Hypotheses

-**Who are the clients eligible for the program of customer loyalty??**
 
Clients with higher average ticket, higher LTV, low recency, higher basket’s size, low probability of churn, higher propensity to purchase?

-**Which percentage of billing per year comes to the Insider Cluster?**

With these data it’s possible to know which is the cost for keeping the Insider Cluster.

-**Revenue expectation:** 

With this it’s possible to plan which actions should be taken to keep the Insider Cluster.

-**Which actions should be taken to make clients with a profile similar to Insider to become one of them?**

**Before applying the model of Machine Learning it’s necessary to identify the pattern of the Insider client through the RFM matrix:**

**Recency:** 

- Time since last purchase;

- Response time of the client.

**Frequency:**

- Average time between the transactions, how much products the client buys in a certain period.

**Monetary:**

- How much does the client bring in revenue?

- Does the client have a higher LTV? 

## Solution strategy

**Data Description:** Rename columuns, Data dimensions, Data types, Replace NA.

**Feature Engineering:** New features have been created through the original features: Gross Revenue, Monetary, Recency, Frequency, Avg Ticket.

**Exploratory Data Analysis:** New features have been created for the validation of business hypotheses, they are:   qtde_invoices, qtde_items, qtde_products,avg_ticket, avg_recency_days, frequency, qtde_returns, avg_basket_size, avg_unique_basket_size.

**Cluster Analysis:** Space study: PCA, t-SNE, Tree-Based Embedding, Decision Tree.

![Tree Based Embedding](https://user-images.githubusercontent.com/77075354/156940453-4dc1037d-6a90-4811-8232-995e7a277897.PNG)

## Top 3 Data Insights

**H1. The customers of Insider Cluster have a volume (products) of purchases more than 10% of total purchases**

**True:** The Insider Cluster has a volume of product purchases of 51%.

**H2. The customers of Insider Cluster have a volume (revenue) of purchases more than 10% of total purchases**

**True:** The Insider Cluster has a revenue of more than 50% of total purchases.

**H3. The GMV of Insider’s customers is concentrated in the third quartile.**

**False:** The revenue of the insider cluster is concentrated on the first quartile.

![Violin Plot](https://user-images.githubusercontent.com/77075354/156940598-654c24ee-be46-46db-b3be-e1d6ee126d3c.PNG)

## Application of Model Machine Learning
Results of Models that have been applied: 

![Resultados do modelos de ML](https://user-images.githubusercontent.com/77075354/156940608-45418c43-ebd0-4bba-95f8-67a73f15af37.PNG)

**For the solution of the problem it has been applied the KMeans:**

![KMeans](https://user-images.githubusercontent.com/77075354/156940643-f3de94b5-568d-49ab-a000-89b7cca1c840.PNG)

## Performance of the Machine Learning Model
![Cluster Validation](https://user-images.githubusercontent.com/77075354/156940689-63ec7c48-fe34-41a5-a551-fa509f0867e3.PNG)

## Business Results

![Clusters](https://user-images.githubusercontent.com/77075354/156941508-52322463-6560-4eac-9096-959959d6e843.PNG)

## Conclusão

Insider Cluster Composition:
- Number of customers: 412 (14% of customers)

- Average revenue: 9.757,00 dollars

- Average recency: 20 days

- Average of products purchased: 451 products

- Frequency of products purchased: 0.10 product/day

- Average revenue: 9.757,00 dollars




