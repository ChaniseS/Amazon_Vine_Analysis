# Amazon_Vine_Analysis
## Overview and Purpose: 
* For this week's project, we will be looking at Big Data and Cloud Services. Big Data is data that has more variety and is generating at high volumes quickly. Spark has become the leading technology for handling big data. This will allow us to process and analyze data quickly and at a massive scale. We will also be using Google Colab since it is hosted in the cloud. This makes it easier to read datasets that are from the cloud as well. Our data will be pulled from Amazon's Simple Storage Service (S3).
* The purpose of this week's project is help businesses optimize their marketing efforts at BigMarket. The project will be to analyze Amazon reviews written by members of the paid Amazon Vine program. Amazon Vine members are delivered products and are required to publish a review. We will be using PySpark to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We will then be using PySpark to analyze our data to determine if there is any bias toward favorable Vine member reviews.

##### For this Project, I chose to Personal Care Appliances dataset:
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Personal_Care_Appliances_v1_00.tsv.gz

## Results:
The dataset had over 85,000 reviews recorded. We took the next steps to zero in on the date:
1. The data was filtered to create a DataFrame where there are 20 or more total votes.
<img width="666" alt="Screen Shot 2022-04-10 at 5 48 27 PM" src="https://user-images.githubusercontent.com/95304025/162641348-9316bc64-c17d-473d-96b4-25d2ae177bfb.png">

2. The data was filtered to create a DataFrame where the percentage of helpful_votes is equal to or greater than 50%.
<img width="666" alt="Screen Shot 2022-04-10 at 5 49 39 PM" src="https://user-images.githubusercontent.com/95304025/162641365-7650e2fd-e6ad-466c-a62b-fb22927fa9a7.png">

3. The data was filtered to create a DataFrame where there is a Vine review.
<img width="666" alt="Screen Shot 2022-04-10 at 5 50 34 PM" src="https://user-images.githubusercontent.com/95304025/162641382-bb31821e-3d37-45f8-b1b6-d92e7cf1c62d.png">

4. The data was filtered to create a DataFrame where there isn’t a Vine review.
<img width="666" alt="Screen Shot 2022-04-10 at 5 51 13 PM" src="https://user-images.githubusercontent.com/95304025/162641399-5cb4d21c-5ac8-4869-8982-fae169a50691.png">

6. The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews were calculated for all Vine and non-Vine reviews.

<img width="888" alt="Screen Shot 2022-04-10 at 5 52 11 PM" src="https://user-images.githubusercontent.com/95304025/162641466-92ac982d-bfa7-493f-ab48-8b1a3d748664.png">
<img width="634" alt="Screen Shot 2022-04-10 at 5 52 20 PM" src="https://user-images.githubusercontent.c<img width="470" alt="Screen Shot 2022-04-10 at 5 52 33 PM" src="https://user-images.githubusercontent.com/95304025/162641485-43c90cd9-013e-4bc3-97f7-60c77bf8da44.png">
om/95304025/162641481-57a5965d-97e6-4add-9707-c499fb2501ed.png">
<img width="470" alt="Screen Shot 2022-04-10 at 5 52 42 PM" src="https://user-images.githubusercontent.com/95304025/162641495-6b1a414e-b311-4210-8684-7cf7cdce6e07.png">
<img width="617" alt="Screen Shot 2022-04-10 at 5 52 55 PM" src="https://user-images.githubusercontent.com/95304025/162641497-1795644d-aab8-4f45-9d61-1849113185ee.png">
<img width="681" alt="Screen Shot 2022-04-10 at 5 53 08 PM" src="https://user-images.githubusercontent.com/95304025/162641508-c6b326e9-96f4-432c-9efe-d2b9f214ffea.png">
<img width="681" alt="Screen Shot 2022-04-10 at 5 53 21 PM" src="https://user-images.githubusercontent.com/95304025/162641510-a726fcd3-cb86-499b-85b8-b36af4857220.png">




