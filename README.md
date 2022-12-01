# Amazon Vine Program Analysis Using PySpark and SQL

## Project Overview
###  
We’ve been tasked with analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I chose to analyze the Digital Ebook Purchase Reviews. Next, I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Then, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.



## Resources
- Data Source: <a href="https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Digital_Ebook_Purchase_v1_00.tsv.gz">amazon_reviews_us_Digital_Ebook_Purchase_v1_00.tsv.gz</a> from the <a href="https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt">Amazon Review datasets</a>, vine_table.csv
- Software: Google Colab, Python 3.7.13, PostgreSQL 14.5, pgAdmin 4 version 6.12, AWS RDS
- Library: PySpark 3.3.1

## Results
How many Vine reviews and non-Vine reviews were there?
- There are 32 Vine (Paid) reviews.
- There are 12,518,670 non-Vine reviews.

<img src="https://github.com/laneyberm/Amazon_Vine_Analysis/blob/main/Resources/images/total_paid_unpaid.png" width="900">

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- There are 17 Vine 5 Star reviews.
- There are 7,678,534 non-Vine 5 Star reviews.

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- The percentage of Vine reviews were 5 stars is 53%.
- The percentage of non-Vine reviews were 5 stars is 61%.

<img src="https://github.com/laneyberm/Amazon_Vine_Analysis/blob/main/Resources/images/percent_5star_total.png" width="900">

What percentage of Vine most helpful reviews were 5 stars? What percentage of non-Vine most helpful reviews were 5 stars?
- There are no Vine most helpful reviews.
- The percentage of non-Vine most helpful reviews were 5 stars is 39%.

<img src="https://github.com/laneyberm/Amazon_Vine_Analysis/blob/main/Resources/images/percent_5star_most_helpful.png" width="900">

## Summary and Recommendations
From the checkout times data, we find that male users are the highest utilizations. Optimizing a marketing strategy to a new bike sharing program should be initally geared towards males. From the user trips by gender and weekeday data, we see that there are higher bike utilization for subscribers for all genders. From the bike maintenance and peak hours data, we see that a majority of the bike utilization is 25% of the bikes. The most ideal time to maintain the high utilized bikes would be from 12am to 5am. 

Recommendations:
- Find the Des Moines population in comparison to NYC. This will help determine the amount of bike to purchase to the intial set up. 
- Find the major transit locations for starting and ending commuters in Des Moines. 

