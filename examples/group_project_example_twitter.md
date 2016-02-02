EXAMPLE: SENTIMENT ANALYSIS OF TWITTER
======================================

OVERVIEW
--------

We continue to see more and more machine learning and analysis tools open up to developers who want to do fun, smart and profitable things with their applications without the effort of rolling their own.  The <a href="http://www.informationweek.com/software/enterprise-applications/ibm-buys-alchemyapi-what-watson-gains-/d/d-id/1319342" title="IBM Buys AlchemyAPI: What Watson Gains " target="_blank">acquisition of AlchemyAPI by IBM</a> should be no shock to anyone, that text analytics is here and here in a big way (see also [HP's IDOL on Demand](https://www.idolondemand.com/), [Aylien](http://aylien.com/) and [LinguaSys](http://linguasys.net/text-analytics) for starters).  Pay very close attention, since the text processing API market over the last few years has been heating up -- and for good reason.  Machines have been marginally good at processing human language, but in the last decade, Natural Language Processing (NLP) technologies have been hoisted by an array of advances in algorithmic techniques as well as platform, infrastructure and hardware advances.  Of course, this has also corresponded with the explosion of human generated data on web, from Facebook and Twitter, to the Blogosphere and beyond.  But no one can read it all, and certainly not consume enough of it fast enough to extract value from it -- unless one has thousands of hours and a large number of humans able to work long hours remain accurate.  Hence, machines to the rescue: from finding out which blogs are talking about the latest cell phones, to Facebook posts that mention the best apple pie recipes or Tweets about last week's episode of The Walking Dead.

## Sentiment Analysis 
At a basic level, sentient analysis is interested in understanding if a text or text fragment can be assigning a sentiment classification -- usually a positive or negative sentiment (and sometimes neutral, if applicable).  While [most journalism strives to be objective](https://en.wikipedia.org/wiki/Journalistic_objectivity), which if successful relays very little personal opinion and tone, it is often very hard to do (though, such objectivity analysis may be worthy of its own). The technical solution to sentiment analysis aims to apply machine learning to determine the tone, opinion, bias or sentiment of a text. A technical introduction to the concepts, algorithms and techniques for performing this type of analysis, can be explored [here](http://sentic.net/sentic-computing.pdf). Furthermore, some popular frameworks for implementing sentiment analysis via NLP tools are [NLTK](http://nltk.org) or [Scikit-Learn](http://scikit-learn.org/). Specific tools that directly implement sentiment analysis are also available, some are language depedent libraries, while others are APIs.

# DATASET
Finding data to explore the sentiment analysis space is generally easy, as there are a plethora of open texts available to both train and test on.  One typical target [Twitter](https://www.twitter.com), is an interesting platform because the data sets can be large and diverse, but more importantly, the 140 character restriction, keeps tweets about to a _sentence or so_ in length.  That makes sentiment analysis easier on the one hand, because the chunks to classify are shorter and in plenitude (for example, analyzing an entire essay for sentiment can be much more complex), but on the other hand presents many issues with the data lacking linguistic structure, sufficient complexity, as well as the language being overloaded with shorthand, odd things like hashtags and other tokens that take up space (URLs) that may not (but could) directly add to assessing the sentiment of the tweet.  Twitter provides an API to extract tweets from which a large dataset will be built.

RESEARCH QUESTIONS
------------------
We're going to explore a test set of tweets about [The Masters golf tournament](http://www.masters.com), specifically tweets which included the hashtag <code>#TheMasters</code>.  On April 12, 2015 during one of the Masters match ups, tweets were collected for a 10 minute window.  In all, 1831 tweets were initially collected (of which 1083 were unique), and the [Tweepy API](https://github.com/tweepy/tweepy) was used for obtaining the data from Twitter.

Our basic questions will first explore:

- What were the characteristics of the tweets in terms of descriptive statistics (unique user count, common users, most common hashtags - excluding #TheMasters)?
- What were the overall sentiment characteristics of the tweets?
- What were the associations of sentiment and other features (hashtags, timestamps, etc.)?
- How well did the classifier built compare to the labeled data - what was the accuracy and performance of the classifier?
- What kinds of features can be used to improve the classifier?

MODELS AND ANALYSIS
-------------------

The models are described and the preliminary analyses were performed in a Jupyter Notebook found in our Github repo under analysis.



CODE AND APPLICATION
--------------------

The code is in Github and instructions on installation are in the README.md file.

PROJECT MANAGEMENT
------------------

Our team consists of two members, Mike C. and Steve G.; Mike did much of the API work, while Stevef did the NLP implementation. API work consisted of building web endpoints to train, test and extract sentiment scores from user supplied texts. NLP work consisted of building a classifier that provided a positive or negative sentiment for a given tweet.

PROJECT DELIVERABLES AND CHECKPOINTS
====================================

| Checkpoint date | Expected Deliverable                                                          | Responsible team member(s) | Checkpoint results                                                                                                                  |
|-----------------|-------------------------------------------------------------------------------|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| 2/1/2016        | Exploratory data analysis of Twitter data.                                        | Mike C., Steve G.          | Basic statistical information about the data; Jupyter notebook of results; cluster analysis of data; code checked in to Github. |
| 2/15/2016       | Development of API  to classify text; endpoints non-functional until classifiers complete                            | Steve G.                    | API testing completed.                                                                                                             |
| 2/29/2016       | Development of classifiers; creation of test and training sets; tuning of classifiers.       | Mike C.                   | API functionality complete; checked in to Github.                                                                                   |
|                 | Development of build and deployment script.  Development of API test harness. | Steve G.                    | Build scripts completed; test cases only at 30% of target (10 tests).                                                               |

(b) TEAM

| Team member | Roles and skills | Contributions |
|-------------|-------------------------|---------------------------------------------|
| Steve G. | API development; testing | Web API implementation; data analysis; test harness; build scripts. |
| Mike C. | Sentiment classifiers; Python | Classifier implementation; data analysis; testing. |