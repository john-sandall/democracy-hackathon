
<img src="https://pydata.org/london2018/static/images/logo.288981a8dfa8.png" alt="PyData London 2019" width="150px"  style="float: left;">


# PyData 2019 Democracy Hackathon: Tweet Challenge


## Description 
- - -
With over 500 members of parliament on Twitter it's a valuable source of direct data from the countries representatives. The goal of this challenge is to harness this information, developing new insights using data available through Twitter's API. 

To get you started we have the most recent 1,000 tweets from every UK politician who operates a Twitter account [(available here)](https://drive.google.com/open?id=1Zh4TpqnDnU9gza6XVlAi4t1G7oYu6J5e), but there are a number of directions you might choose to take.


Some establish political twitter projects include:
 - [MP's on Twitter: Aggregate statistics, most mentioned users and hashtags etc.](https://www.mpsontwitter.co.uk/) 
 - [Politiwoops: MP's deleted tweets](https://www.politwoops.co.uk/p/ukmps)
 
And some examples of analysis using twitter data:
- [BBC: Which MPs don't display party allegiance on Twitter?](https://www.bbc.co.uk/news/uk-politics-42778241)
- [Portland communications: House of Tweets: Understanding the social networks of MPs](https://portland-communications.com/2017/10/26/house-of-tweets/)
- [Commons Library: The use of Twitter by MPs in parliamentary debate](https://commonslibrary.parliament.uk/insights/the-use-of-social-media-by-mps-in-parliamentary-debate/)



## What's available through the API
---
In the 'Using Twitter API to build a dataset notebook' you will find the code for making an API call on a Twitter users timeline. This API is set up to collect the following information:
- User
- Tweet time
- Location (if available)
- Hashtags
- Source device
- Tweet text 
- Retweet text (if retweet, contains full text - 'tweet text' is truncated if retweet and over 140 characters)
- Quote text (if quote)
- Quote screen name
- Status count (number of tweets to date)
- Favourite and retweet count (at time of call)

The 1,000 tweets available in the csv have been made using the call function in the Twitter API notebook so will have this information available.

[Tweepy](http://docs.tweepy.org/en/latest/) is used to interact with Twitter's API.

See here for a full list of [Twitter API calls](https://developer.twitter.com/en/docs/api-reference-index.html).


## Ideas to get you started
- - -
#### Perform analysis on the existing data set
- Sentiment analysis of tweets by party/topic/constituency using [NLP libraries](https://elitedatascience.com/python-nlp-libraries)
- Frequency of tweets by topic or key words (over time)
- Network analysis - who retweets who and what can it tell us?
- Retweet favourite counts - which politicians and topics get the most traction

Depending on how you choose to visualise your data, there may be a large number of data points in your plots. The [Plotly library](https://plot.ly/python/getting-started/) provides interactive visualisations that allow for zooming that maintains the resolution of plots. [This article](https://towardsdatascience.com/the-next-level-of-data-visualization-in-python-dd6e99039d5e) is a great starting point for users new to Plotly.

#### Acquire more data and analyse that
- API calls on large datasets can take a while, but if you are interested in just a few users you can use the call function to acquire their most recent 3,200 tweets in a relatively short time. 
- We already have a list of MP's twitter username, but there are other groups (for example journalists) that we may want to analyse in future, can you identify a group and collect screen names and user id's for future analysis. [This article](https://towardsdatascience.com/use-google-and-tweepy-to-build-a-dataset-of-twitter-users-cbfd556493a9) details how you can use a different API call to collect existing twitter lists that feature key words.

#### Scale up
- How can we improve on or create new projects like politwoops and MP's on twitter that provide valuable up to date information on the activity of politicians and associated groups. What assets would be needed to sustain such a project?

