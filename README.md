<img width="526" alt="image" src="https://user-images.githubusercontent.com/94858846/164155629-da52ece0-d289-4249-9201-6f80a05ed306.png">


# Amazon_Vine_Analysis
Big data and AWS

## Purpose

In today's competitive market, buyers often rely on reviews they find before buying any product.The purpose of conducting this analysis was to investigate any bias towards reviews written as part of Amazon's Vine program, a paid program, and regular consumers from a dataset. The below "selected dataset for analysis" was chosen from approximately 50 datasets and ETL was performed. 


## Resources:
**Data Source:** [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) </br>
**Selected dataset for analysis:** [Lawn and Garden](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Lawn_and_Garden_v1_00.tsv.gz) </br>
**Softwares and applications:** Google Colab, PostgreSQL, pgAdmin, AWS, PySpark

## Results:
1. The dataset was extracted as a datframe </br> <img width="1051" alt="image" src="https://user-images.githubusercontent.com/94858846/164254988-d2b7e1c8-b78c-4479-afe2-ff0c43a9383e.png">

2. The extracted data was then filtered with only selected data necessary for this vine review analysis. A minimum number of votes(=20)was selected to pick reviews that are more likely to be helpful and to avoid having division by zero errors later on.</br> <img width="598" alt="image" src="https://user-images.githubusercontent.com/94858846/164254692-08de6782-451a-4319-95c3-2b203f76798e.png">

3. The dataframe was then further filtered where helpful votes form the 50% of the total votes. </br> <img width="772" alt="image" src="https://user-images.githubusercontent.com/94858846/164254878-44eaaddf-b811-443d-9ade-34d3ffe8f93e.png">

4. Lastly the data was filtered to show the vine and non-vine reviews count and percentage which shows the bias.</br> <img width="646" alt="image" src="https://user-images.githubusercontent.com/94858846/164255227-bfe466a2-d056-4fea-b5af-1ef9f093a363.png">
</br> <img width="796" alt="image" src="https://user-images.githubusercontent.com/94858846/164255311-30a8fabc-f923-40a0-82c0-a141e73130d4.png">

5. Below is the summary showing the calculated vine and non-vine reveiws + 5-star reviews, vis-a-vis total reviews -</br>  <img width="740" alt="image" src="https://user-images.githubusercontent.com/94858846/164254282-51c58d9c-e128-41c8-9d30-eed963465262.png">

## Analysis Summary: 
- It was analysied that contributing helpful vine 5-stat reviews form almost negligible proportion of reviews = 0.01%
- With that being derived, it is evident that **this dataset for Lawn and Garden equipment is not biased towards vine(or paid) reviews** and it is the honest reviews (5-star reviews or below) that are available on portal and will hence provide unbiased opinions for a particular equipment or merchandise 



