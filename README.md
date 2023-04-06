# We Rate Dogs # 🐶

## WeRateDogs is a popular Twitter account with 9.3 million followers that rates people's dogs with a humorous comment. 

This is a description of the project.

#Data Wrangling Report Gathering:

1. The WeRateDogs Twitter archive was downloaded manually from Udacity (twitter_archive_enhanced.csv) and saved as a data frame (archive).
2. The tweet image predictions were downloaded programmatically using the requests library, using the URL: https:// d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image- predictions/image-predictions.tsv and saved to image_predictions.tsv and loaded to a data frame (predict).
3. Additional data from the Twitter API was queried by Twitter API and each tweet's JSON data using the Tweepy library and stored as tweets' entire set of JSON data in a file called tweet_json.txt file. A data frame (twitter_api) was created including only ['tweet_id', 'retweet_count', 'favorite_count'].
4. All three data frames were merged into one data frame called df_final for assessment.

