# Amazon Vine Analysis
 An analysis of Amazon product reviews using PySpark, Python, and Postgresql
## Project Overview
The Amazon Vine program is an invite-only program which gives a select number of individuals the opportunity to receive free product in exchange for reviews. This project analyzes the Amazon Vine program and evaluates potential bias toward favorable reviews from Vine members. <br><br>Google's Colaboratory notebooks, in conjunction with PySpark, were used to perform the Extract, Transform, Load (ETL) method by extracting the initial data, transforming the data, connecting to an AWS RDS instance, and loading the transformed data into a PostgresSQL database instance. Additional analysis was done using a Google colaboratory notebook and PySpark. <br>


## Resources
<b>Data Sources:</b><br>
- Amazon Review Dataset: Amazon apparel review dataset found [here](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)<br>

<b>Software:</b><br>
- Google Colaboratory Notebooks<br>
- PySpark 3.2.2<br>
- AWS RDS<br>

## Results

![Amazon_Vine_Analysis_Bias_Calculations](https://user-images.githubusercontent.com/105830645/199640056-23722306-7c49-405d-808b-78957d1add5f.png)
<br><br>
<b>1. How many Vine reviews and non-Vine reviews were there?</b>
- Number of Vine reviews: 33
- Number of non-Vine reviews: 45388

<b>2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?</b>
- Number of Vine 5-star reviews: 15
- Number of non-Vine 5-star reviews: 23733

<b>What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?</b>
- Percentage of Vine reviews that were 5-stars: 45.5%
- Percentage of non-Vine reviews that were 5-stars: 52.3%

## Summary
From this analysis there is no demonstrable bias towards 5-star reviews for participants in the Amazon Vine program. However, the sample size of Vine reviews is quite small. A larger sample size of reviews across several product categories would be required to positively conclude no bias exists. Recommendations for further analysis include examining multiple categories and performing similar analysis for each. Also, determining the distribution of 1,2,3,4, and 5-star reviews from reviewers in the Vine program and comparing this distribution to non-Vine reviewers should be done to better understand how receiving paid product may impact review scores.
