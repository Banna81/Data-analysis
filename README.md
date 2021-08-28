# Data-analysis
Collecting and Investigating 3 datasets about tweets of dogs pictures that are rated about how cute they are  
The data is collected from Twitter API for the tweets, json file describing the prediction of the dogs breeds.
Gathering:
- Well for the first two datasets Twitter-archive and image predictions I downloaded them manually and the third one using twitter API and storing the data in tweet-json.txt as per the project guide
- I needed to have the ratings with the breeds in one dataset and that required some work as the image predictions dataset was read as one column and the same for tweet json, the separators couldn’t be identified.
- So I used regular expressions after taking closer look at them by .head and .info
- I fixed the variation of white spaces as separators in image predictions by using the right regex (one space or more )as delimiter.
- I used read_json for the json file after I changed the extension of it.
- Now the three datasets are ready to be communicated with. I started working on merging the first two datasets using join and matching the tweet_id in both, but that required me to change the column name in one of the data frames.
- Finally, I saved the two data frames of the first two data sets in one .csv file and the third data frame in another .csv file.
Assess:
- I loaded the two new datasets to two data frames and used .info .head .describe to discover them.
- I counted the unique values in the important columns.
- I checked the number of single character in the names column.
