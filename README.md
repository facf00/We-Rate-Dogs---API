# 🐶 We Rate Dogs 🐶

## WeRateDogs is a popular Twitter account with 9.3 million followers that rates people's dogs with a humorous comment. 

This is a description of the project.

#Data Wrangling Report Gathering:

* To analyze the WeRateDogs Twitter account, we needed to gather data from different sources. First, we downloaded the WeRateDogs Twitter archive file (twitter_archive_enhanced.csv) manually from Udacity and saved it as a pandas DataFrame called "archive". This file contains data about each tweet, such as its text, timestamp, and rating.

 * Next, we downloaded the tweet image predictions file using the requests library. We used the following URL to download the file programmatically: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv. The file was saved as "image_predictions.tsv" and loaded into a pandas DataFrame called "predict". This file contains information about the images in the tweets, including their URLs and predicted dog breed.

* We also wanted to collect additional data about each tweet, such as the number of retweets and favorites. To do this, we used the Tweepy library to query the Twitter API for each tweet's JSON data. We stored the entire set of JSON data for each tweet in a file called "tweet_json.txt". We then extracted the desired data fields (tweet_id, retweet_count, and favorite_count) from the JSON data and created a pandas DataFrame called "twitter_api".

 *Finally, we merged the three data frames ("archive", "predict", and "twitter_api") into one DataFrame called "df_final" for assessment. This allowed us to perform data cleaning, quality assessment, and exploratory data analysis on the combined data set.