# WeRateDogs Wrangling_Project

## Data Wrangling Process
In this project, I performed wrangling processes of a Twitter account to make the data clean and ready for analysis.

- Data Gathering
- Data Assessing
- Data Cleaning

### Quality issues

##### df_archive table
- The following columns ('name', 'doggo', 'floofer', 'puper', 'puppo') all had their empty cell filled as None instead NaN.
- Dog Name column have invalid names like 'None', 'quite', 'such', 'the 'a', 'an'.
- Erroneous datatypes
- Some rating_denominator are not equal to 10.
- Invalid values found in rating_numerators columns.
- duplicated values found in expanded_urls column.
- Reduce breed Predictions columns to two column only (dog_type and confidence_level).
- Some data are retweets but we only want to keep “original tweets”, no “retweets”.
- Reply tweets are not “original tweets” either.
- Delete columns not needed for analysis.

##### df_tsv table
- Duplicates rows exists(some rows have duplicates in every column except the tweet_id column)
##### df_jason
- drop Create_date column.


### Tidiness issues
- Dog stages (doggo, floofer, pupper, puppo) are spread in different columns.
- Create_date exists already in df_archive, we need it in only one of the dataset.
- Merge all three dataset to one table

## Analysis and Visualization of Data
- What is the most popular dog type?
- What is the most popular dog stage?
- most used device for tweeting (source)
- Dogs ratings to retweet counts
- correlation between retweet count and favorite count?
