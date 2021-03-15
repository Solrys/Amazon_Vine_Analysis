# Amazon_Vine_Analysis

## Background

For this project I will be analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

For this project, I had access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I chose "Video Games" and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afte that I used PySpark once again to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

## Method

* PYSPARK
* JUPYTER NOTEBOOK
* GOOGLE COLLAB
* SQL
* AWS

## Overview of the Analysis:

In order to closely Analyze the datasets after I have Extracted and Transformed the reviews for Video Games I Wanted to focus on the following questions:

1) How many Vine reviews and non-Vine reviews were there?
2) How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
3) What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

## Results:

1) There are a total of 40,565 reviews. 
94 vine reviews and 40,471 are non-vine reviews. 
The small percentage of vine reviews is important to consider while moving forward with this analysis. 
![image](https://github.com/Solrys/Amazon_Vine_Analysis/blob/main/images/Screen%20Shot%202021-03-14%20at%2011.23.02%20PM.png)

2) There was a total of 15,711 5-star reviews with 48 5-star vine reviews and 15663 5-star non-vine reviews.

3) Finally 51.06% of paid reviews are 5-stars and 38.7% of unpaid reveiws are 5-stars.


![image](
![image](

## Summary:

After looking that the results, I would conclude that there is a positivity bias for reviews in the Vine program. It is important to note that while the non-vine sample size was very large, the vine sample size was less than 100 entries. While 94 entires is still a decent number to sample with, it could lead a less signifcant result. In addition to the current analysis, I could take it a step further and see the percentage of those who purchased the product by filtering through the verified_purchase column to either confirm or fail to confirm if there is a positivity bias for reviews in the Vine program.
