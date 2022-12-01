# Amazon Vine Program Analysis Using PySpark and SQL
PySpark, Pandas, SQL, pgAdmin, AWS RDS

## Project Overview
###  
Investors want to know if they should invest in a citibike sharing venture in Des Moines, Iowa. The core issue we need to think about is what we absolutely need to know in order to create our bike-sharing program in Des Moines. We will use data analysis of New York City Citibike Data from August 2019 to collect information for the investors prior to opening this new business. 

Questions they have include: how many bike trips were recorded during the month of August(beautiful time of the year to rent a bike), number of short-term customers and annual subscribers to the Citi Bike service, peak hours for bike rentals, highest-traffic locations, top locations for starting a bike journey, rider data regarding gender, average duration of a bike ride, and key costs including initial set up and bike upkeep through maintenance.

## Resources
- Data Source: <a href="https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip">201908-citibike-tripdata.csv</a> from the <a href="https://ride.citibikenyc.com/system-data">Citi Bike System Data page</a>
- Software: Jupyter Notebook 6.4.8, Python 3.7.13, Tableau Public 2022.3.0
- Library: Pandas 1.3.5

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

