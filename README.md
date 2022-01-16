# Ecommerce_Customer_Segmentation
Statistical Learning Project Unsupervised Learning

#The Dataset In this project, we will utilize the Brazilian E-Commerce Public Dataset made at Olist. Olist Store is a Brazilian e-commerce marketplace integrator that concentrates the products of all individual sellers to the consumer. Currently, the company has 300 employees, more than 9000 shopkeepers, and 2 million consumers. the dataset has information of over 100 thousand orders from 2016 to 2018. The dataset is a collection of several subsets that contains information on customer location, product attributes, order status, expense, payments, as well as geolocation information. We will combine these subsets in the data-wrangling state.

#The Research Question By taking advantage of these well-organized datasets, we aim to explore and predict yearly sales data using consumer cohorts and product-categories-related data as predictors. Using unsupervised statistics learning algorithms allows us to extract features from the datasets that normal statistical methods might not be able to see. Specifically, we want to first use k-means clustering to divide all consumers into several consumer groups, then explore the relationships between the product sales, their respective consumer groups composition. In the project, we will first use exploratory graphs and geography maps to visualize the inherent consumer cohort structure Then, using the newly created groups as features, we will apply two supervised learning algorithms - kNN and Random Forest - to predict yearly sales. We will also comment on the transferability of our model, after doing some optimization and efficacy evaluation.

# Interpreting Customer Clusters 

From the loaded dataset, we are able to obtain information on the orders information related to a specific customer identified by a specific customer_id. Furthermore, we are also able to collect the general geographic location related to a customer. Interesting behaviors can be observed from the dataset. When looking at the first 6 observations of the customer.final data frame, for example, we can see that the same customer frequently buys the same item with a price tag of 89.9. And We could gain some insights on this specific customer id when we know what this item actually is. And by merging the two datasets together we are set up to the dataset for k-means clustering analysis. We now apply the k-means clustering method to divide our consumers into 6 groups. The k-means clustering method aims to partition n observations into k clusters. The method that will use to classify each observation is using the mean of the cluster centroid. We feel like this dataset would be a great opportunity to apply k-means clusters since different customers with similar personal, psychological, social, geographical backgrounds often share similar behavior when they purchase any item. So, instead of treating each customer as an individual we think treating customers as groups will not only generate more meaningful insights but also create more applicable algorithms to predict the sales based on the cohort size.

<img width="548" alt="Screen Shot 2022-01-16 at 12 06 56 AM" src="https://user-images.githubusercontent.com/93837295/149648070-fe7bf39b-3f8b-4c59-9064-4dee1cf8faee.png">

<img width="685" alt="Screen Shot 2022-01-16 at 12 07 44 AM" src="https://user-images.githubusercontent.com/93837295/149648083-075b8f20-a798-4651-b089-d640fa9220cf.png">

<img width="462" alt="Screen Shot 2022-01-16 at 12 08 08 AM" src="https://user-images.githubusercontent.com/93837295/149648089-362abaf3-40d2-434d-85f3-d1a709ae7976.png">

<img width="486" alt="Screen Shot 2022-01-16 at 12 09 08 AM" src="https://user-images.githubusercontent.com/93837295/149648106-39d2583c-543f-4c4d-a488-f123bf641749.png">

# Predicting Sales

In this project, we will test the efficiency of the “after” part of the Brazilian E-Commerce Public Dataset made at Olist. The whole dataset consists of information of over 100 thousand orders from 2016 to 2018 and we extracted only the only from 2017-2018 as our “after” data and utilized the before model to compare the predicted values and actual values. Again, the ordered dataset is a collection of several subsets that contains information on customer id, product attributes, order status, payments, as well as product and category information. We will combine these subsets in the data-wrangling process to match the order of before the process

<img width="708" alt="Screen Shot 2022-01-16 at 12 11 42 AM" src="https://user-images.githubusercontent.com/93837295/149648162-8ea507fc-c337-4463-a45c-b8a55c4162c1.png">

<img width="699" alt="Screen Shot 2022-01-16 at 12 12 12 AM" src="https://user-images.githubusercontent.com/93837295/149648177-427eca0b-85d2-4c4b-b62b-1fb869a33495.png">

<img width="720" alt="Screen Shot 2022-01-16 at 12 12 27 AM" src="https://user-images.githubusercontent.com/93837295/149648185-2b58741d-229c-486e-94c0-953b8353559b.png">

<img width="679" alt="Screen Shot 2022-01-16 at 12 12 44 AM" src="https://user-images.githubusercontent.com/93837295/149648193-8bf84462-b334-4e25-8555-13ce336b556f.png">

