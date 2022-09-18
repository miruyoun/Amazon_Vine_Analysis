# Amazon Vine Analysis

## Overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products in exchange for paying a fee to Amazon so they can distribute the products to their members. In this analysis, I analyzed game reviews written by members of the paid and non-paid Amazon Vine program. Additionally, I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Finally, I used Pandas, to determine if there is any bias toward favorable reviews from Vine members in my dataset.

## Results
  * How many Vine reviews and non-Vine reviews were there?
  
  ![total1](https://user-images.githubusercontent.com/106292020/190878824-1dad991c-0412-4112-9d85-52a98fa47331.PNG)
  ![total2](https://user-images.githubusercontent.com/106292020/190878826-20da7b64-806e-4f6b-b239-88b889896467.PNG)
  
  There are 94 Vine reviews and 40,471 non-Vine reviews.

  * How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  
  ![percent1](https://user-images.githubusercontent.com/106292020/190878834-6a8903f0-db13-4ada-bd1e-0e405c368c21.PNG)
  ![percent2](https://user-images.githubusercontent.com/106292020/190878833-4128a188-2f74-4d72-b623-7cc6adb4592f.PNG)
  
  There are 48 Vine reviews that were 5-star and 15,663 non-Vine reviews that were 5-star.

  * What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  
  ![prop1](https://user-images.githubusercontent.com/106292020/190878837-e01657c3-6d92-45bf-9813-f55e5870485d.PNG)
  ![prop2](https://user-images.githubusercontent.com/106292020/190878838-cda728be-9436-4fe3-aee8-2e927e087a4d.PNG)

  Around 51% of Vine reviews were 5-star and around 39% of non-Vine reviews were 5-star.
  
## Summary
There seemed to have been some kind of bias because the proportion of 5-star reviews was significantly higher in Vine reviews than non-Vine reviews. There was about 10% difference in Vine and non-Vine reviews. A product having more than 50% 5-star reviews is very unlikely and people that are given free or cheap products will more likely to give higher ratings.
To further study this analysis, I would need to see the other star ratings so that I can see if the distribution of rating is even or skewed.
