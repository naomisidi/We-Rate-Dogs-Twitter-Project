# We-Rate-Dogs-Twitter-Project
The WeRateDogs Twitter gathers data from a local file, programmatically from Udacity servers and by querying the Twitter API, merges the three datasets into one dataframe, conducts visual and programmatic assessment to check its quality and tidiness, then clean it. The clean data is then used to provide worthy analyses and visualizations

## Introduction
This project focused on the wrangling part of the Data Analysis process. The goal was to use WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog that has over 9 million followers and has received international media coverage. Although the ratings have a denominator of 10, the numerator is almost always greater than 10 for instance 12/10, 13/10, and so on. This forms part of WeRateDogs unique and often humorous dog rating system.

## Summary of Findings

### Quality Issues
* Validity: Some tweet_ids represent retweets and not original tweets
* Some tweet_ids represent replies and not original tweets
* Name column in enhanced dataframe contains inaccurate values (e.g. a, none)
* The text column of the enhanced dataframe contains both tweets and tweet url
* The enhanced dataframe expanded url column contains the same information as the url substring in the text url
* The enhanced dataframe source column contains the actual source and html code
* Timestamp column in enhanced dataframe is in string format
* Non-descriptive column names in the enhanced and image-predictions dataframes
* Dog Prediction, Confidence level and Breeds are contained in three different columns. 324 rows are predicted false, not related to dogs.

### Tidiness Issues
* Data describing age/stage of the dogs (doggo, flooffer, pupper, puppo) contained in different columns in enhanced dataframe
* The data is contained in 3 different tables with duplicated column names

## Cleaning Data
This process involved cleaning all issues using pandas, numpy and regular expressions.
