# Amazon_Vine_Analysis

## Analysis Overview
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.\
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.\
We focused on the US reviews for video games.

## Resources
- Data Source: [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), [Video Games Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
- Software: Google Colab Notebook, pgAdmin 4, AWS

## Results
### Total number of reviews
- Vine reviews <p align="center">
    <img src="https://user-images.githubusercontent.com/68669675/99216761-18d62180-279c-11eb-9190-f5af7b8039ad.png"> 
</p>

<br>

- Non-Vine reviews <p align="center">
    <img src="https://user-images.githubusercontent.com/68669675/99216760-17a4f480-279c-11eb-87a8-733eb08893d7.png"> 
</p>
<br>

### Total number of 5-star reviews
- Vine reviews <p align="center">
    <img src="https://user-images.githubusercontent.com/68669675/99217107-e678f400-279c-11eb-9523-a2f5ef938070.png"> 
</p>

<br>

- Non-Vine reviews <p align="center">
    <img src="https://user-images.githubusercontent.com/68669675/99217109-e7118a80-279c-11eb-93e8-4ea595a723e2.png"> 
</p>
<br>

### Percentage of 5-star reviews
- Vine reviews <p align="center">
    <img src="https://user-images.githubusercontent.com/68669675/99217345-77e86600-279d-11eb-89ce-5704117874da.png"> 
</p>

<br>

- Non-Vine reviews <p align="center">
    <img src="https://user-images.githubusercontent.com/68669675/99217349-79199300-279d-11eb-826d-18001d7e6b68.png"> 
</p>
<br>

## Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.\
Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.