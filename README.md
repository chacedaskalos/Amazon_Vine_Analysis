# Amazon_Vine_Analysis

## Overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Results
* How many Vine reviews and non-Vine reviews were there?
There were 90 Vine reviews and 37831 non-Vine reviews

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
44 Vine reviews were 5 stars, 14704 non-Vine reviews were 5 stars

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
48.89% of Vine reviews were 5 stars, 38.87% of non-Vine reviews were 5 stars

![analysis](https://user-images.githubusercontent.com/96211484/163656497-4cc32531-87ee-43f0-a760-541470b105e3.png)

## Summary 
It appears there is an advantage to using the Vine program as Vine reviews got 10% more 5 star reviews, but it is important to also be cautious and look at the sample size. There is only 90 Vine reviews and 37831 non-Vine reviews so the data can be skewed. A further analysis that can be run is looking at 1 star reviews to see if Vine program raises the "floor" on bad reviews.
