# bidnamic-data-challenge
Bidnamic's Data Engineering Coding Challenge 


Please find my solution to the Coding Challenge [here](https://github.com/akhilnarala/bidnamic-data-challenge/blob/master/bidnamic-data-challenge-akhilnarala.ipynb)

## Practices I used to solve this problem 
1. As a first step toward addressing the problem, I connected to AWS S3 and created Buckets dynamically by prefixing the Bucket name with the current Unix timestamp, ensuring that no two buckets created are identical. 
2. The data from the Google Ads API must then be transferred to the AWS S3 Data Lake. The code for connecting to S3 is in the aforementioned ipynb file. 
3. Pyspark was used to retrieve data from AWS S3 and load it into DataFrames. 
4. The Pyspark DataFrame Transformations are used for data preprocessing. 
5. As a further step, developed a Final DataFrame that includes the Return On Ad Spend (ROAS) for each search phrase.
6. The resulting DataFrame is then placed in a PostgreSQL database hosted by AWS Services.
7. Businesses may simply query aggregations on the final table using simple SQL commands, as demonstrated at the conclusion of my solution in the ipynb file.
