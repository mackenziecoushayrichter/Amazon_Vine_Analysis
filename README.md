# Amazon Vine Analysis
## Overview of Analysis
* The purpose of this analysis was to access a large dataset of amazon reviews for a certain type of products, and determine if there was any bias towards favorable reviews. 
* To determine this, I looked into the dataset to see which reviews were written by Vine program members.
* The Amazon Vine Program is a program where Amazon pays members of the program to write reviews for different products.
* I used Pyspark to perform the ETL process on the dataset and connected it to an AWS RDS instance
* Then I loaded the transformed data into PgAdmin.
* Finally I used Pyspark to perform my final analysis
## Results
* After performing my analysis I found the following results:
  * There were 37,993 total reviews.
  * 170 of those reviews were part of the Vine Program, 37,823 were not part of the vine program.
![](images/total_reviews.png)
 * Out of the 37,993 reviews, there were 20,670 five star reviews
 * 65 of the 5 star reviews were part of the paid Vine Program, 20,605 of the 5 star reviews were not part of the paid Vine Program
 ![](images/five_star_reviews.png)
 * 38% of the reviews from the paid Vine program were 5 stars
 ![](images/vine_five_star.png)
 * 54% of the reviews that were not part of the Vine Program were 5 stars
 ![](images/no_vine_five_star.png)
 ## Summary
 * From my analysis I found that there is not a positvity bias for reviews that were a part of the paid Vine Program, as only 38% of these reivews gave the product 5 stars
 * This is compared to the reviews that were not a part of the paid Vine Program 54% of those reviews gave the product 5 stars
 * To furthur my analysis with this dataset, I also found the percent of paid five star reviews and unpaid five star reviews from the total number of 5 star reviews
 * There were 20,670 total five star reviews.  65 of those were paid, and 20,605 of those were unpaid.
 * Meaning that 99.7% of the Five Star Reviews were unpaid
 ![](images/five_star_percent.png)
 
