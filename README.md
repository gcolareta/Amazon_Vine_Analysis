# Amazon_Vine_Analysis

## Overview
In this project I am analyzing Amazon reviews written by members of the paid Amazon Vine program. Amazon Vine program is a service that allows companies to receive a review for their product by paying a small fee to Amazon and providing products to Amazon Vine members who are required to post a review on the product.

In this analysis of product reviews, I am hoping to determine if there is any bias toward favorable reviews from Vine members in this dataset.

## Results
From the approximately 50 datasets I had access to, I selected the following one:
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Shoes_v1_00.tsv.gz

The dataset was filtered to only account for the most significant reviews based on the number of helpful_votes.

Since the purpose of the analysis was to determine if the reviews of the Vine members were biased, I considered only the five-star reviews and compared the percentage of the paid 5-star reviews against the percentage of unpaid 5-star reviews.

The results indicate that less than 1% of Vine members gave a 5-star review to the product category selected (shoes). Thus, more than 99% of non-paid reviewers gave a 5-star review.

The following is a summary of the results:

-	We evaluates 27,009 reviews in total

<img width="1146" alt="vine_df" src="https://user-images.githubusercontent.com/104762216/191850247-fb9d9a0d-919c-443d-96ff-56f45494164c.png">
<img width="314" alt="total_reviews_count" src="https://user-images.githubusercontent.com/104762216/191850263-9e5b9e66-5ca6-43a3-8783-b58610280233.png">

- From the total reviews, 22 were from Amazon Vine members.

<img width="732" alt="Screen Shot 2022-09-22 at 5 06 43 PM" src="https://user-images.githubusercontent.com/104762216/191851169-b2f535ce-f467-4d8f-813e-0f3e0e237aa9.png">
<img width="607" alt="Screen Shot 2022-09-22 at 5 06 52 PM" src="https://user-images.githubusercontent.com/104762216/191851178-e29277a1-130c-4b29-bdfd-965713343d04.png">

- 26,987 reviews were from non-Vine members
<img width="723" alt="Screen Shot 2022-09-22 at 5 09 27 PM" src="https://user-images.githubusercontent.com/104762216/191851633-6ca46908-1441-4a81-bbe7-4098277f2495.png">
<img width="625" alt="Screen Shot 2022-09-22 at 5 09 34 PM" src="https://user-images.githubusercontent.com/104762216/191851699-f5109666-8792-4ffd-a3e9-e0889345a222.png">

- The total 5-star reviews was 14,488 (53.6% of reviews). Out of those, only 13 (0.09% of 5-star reviews) were done by Vine members. 14,475 (99.91% of 5-star reviews) were from non-vine members.


## Summary
There is a limited amount of reviews from Amazon Vine members in this particular dataset. Based on this data, it seems that members of the Vine program do not give biased reviews. However, with the proportions of member versus non-menber reviews in this dataset, this conclusion cannot be reached. I would like to analyzed other datasets to have a more accurate sample data.



