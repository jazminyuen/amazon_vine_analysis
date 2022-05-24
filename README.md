# Overview 
Analyze Amazon product reviews of musical instruments written by members of the paid Amazon Vine program to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Resources:
- Amazon Web Services (AWS), Relational Database Service (RDS)
- PostgreSQL 11, pgAdmin 4 Version 6.4
PySpark Version 3.2.1
- Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Musical_Instruments_v1_00.tsv.gz

## Results: 

- In this dataset, there are 14,477 non-Vine reviews and 60 Vine reviews.
- Of the five-star reviews, 8,212 are non-Vine and 34 are Vine.
- 57.7% of non-Vine reviews are five-star, and 56.7% of Vine reviews are five-star.

![Unpaid Stats](/images/unpaid_stats.jpg)

![Paid Stats](/images/paid_stats.jpg)



## Summary: 

- In this analysis, we are comparing the percentage of five star reviews written by members of the Vine program who are paid for their reviews to the percentage of five star reviews written by those who are not paid for their opinion.

- Since the results of our analysis show that this metric is nearly the same number, we can state that there is no positivity bias for reviews in the Vine program within this dataset.

- To further investigate our primary question, we can parse the text in the body and title of the reviews to see if there are similarities amongst the Vine reviews. Additionally, we can observe the frequency of reviews and star ratings by customer ID.