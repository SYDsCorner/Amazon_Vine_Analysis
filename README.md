# Amazon_Vine_Analysis

<p align="center">
  <img width="800" height="274" src="https://user-images.githubusercontent.com/89308251/145699265-b1595efd-eb0d-41b1-9200-40972c360b0f.jpg">
</p>

## Challenge Overview

### Purpose:

   The purpose of this analysis is to use PySpark to perform the ETL process to extract one of the datasets from Amazon reviews written by members of the paid Amazon Vine program. To accomplish this I transformed the data, connected to an AWS RDS instance, loaded the transformed data into pgAdmin, and then used PySpark to determine if there was any bias towards favorable reviews from Vine members in the dataset.
  
  
## Resources
- Software:
   - [Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb) (Google Colab Notebook)
      - PySpark 
   - [Amazon Web Services (AWS)](https://aws.amazon.com/)
   - PostgreSQL 12
   - pgAdmin 4 

   
- Data source: 
   - Amazon Review datasets 
      - [Amazon Furniture Reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Furniture_v1_00.tsv.gz)

## Results 

<p align="center">
  <img width="503" height="119" src="https://user-images.githubusercontent.com/89308251/145699945-81ec2299-0f10-4062-ad89-76aec46dbcc4.png">
</p>
  
  
- The **total number** of reviews for all **Vine** and **non-Vine** reviews 
   > ![total_number_reviews](https://user-images.githubusercontent.com/89308251/145699865-ddead52d-3db2-4daf-bf20-c3486f607e8a.png)

   - The total number of reviews for all Vine and non-Vine reviews is 18,155 people.
      - Appoximately **1%** are **Vine** members. (136 people)
      - Appoximately **99%** are **non-Vine** members. (18,019 people)


- The number of **5-star reviews** for all **Vine** and **non-Vine** reviews 
   > ![number_5star_reviews](https://user-images.githubusercontent.com/89308251/145699885-1150b533-a326-4ed0-8d94-2af75bb93ea8.png)

   - There **74** out of 136 **Vine** members gave 5-star reviews.
   - There **8,482** out of 18,019 **non-Vine** members gave 5-star reviews.


- The **percentage 5-star reviews** for all **Vine** and **non-Vine** reviews 
   > ![percent_5star_reviews](https://user-images.githubusercontent.com/89308251/145699886-11e293bf-bf25-4613-a1e3-756ebea9da25.png)

   - Appoximately **54%** of **Vine** members gave 5-star reviews.
   - Appoximately **47%** of **non-Vine** members gave 5-star reviews.


## Summary:   

For the results, we could come to the conclusion that there is a **positivity bias** for reviews in the Vine program on the **furniture category**. 
However, there are more than 50 datasets and difference categories that we could use to prove even further if there is any bias towards favorable reviews from Vine members.

- The additional analyses that we could do with this dataset to support our statement are 
   - use more datasets that are different categories from the Amazon Review datasets.
   - analyze more summary statistics such as mean, mode, and median of the star rating.

