---
layout: default
---

## BLOG
In this blog, I want to start sharing my journey through [the age of the algorithm](https://maisonneuve.org/article/2011/05/9/age-algorithm/) and take the time to publish some of the ways in which I work with data in my day to day life.

<br>

### What have I been tweeting? (written on 12/17/2017)
I've been [tweeting](https://twitter.com/megmfurr) since February 2015 when I was in [UVA's Data Science Institute](https://dsi.virginia.edu). Recently, with my twitter data, I've been wanting to do data science work.

Today, I started out by collecting and storing my twitter data.

First, I import [tweepy](http://www.tweepy.org), a Python module/library that supports gaining access to twitter data. I use a function defined by someone else online, shared on [git](https://gist.github.com/yanofsky/5436496), and pull the most recent data and am able to pull over 2,529 going back to February 22, 2015.

<img class="picture" src="get-all-tweets.jpg">
<img class="picture" src="getting-tweets.jpg">

Some examples of the tweets in the csv file written out are the following: 

<br>
(1) "RT @dpatil: This is what I mean when I say data scientists are the new first responders -- new tech to help those in need and augment the t‰Û_"
<br>
(2) "RT @UVADSI: Data scientists are changing the nature of employment, and the meaning of employability @ftdata https://t.co/WFl2tKCWnG"
<br>
(3)"I published some #thoughts &amp; #questions "My Journey from History to Data Science‰Û https://t.co/Sh9rzqOONC #Humanity #Data #Tech #Kindness"
<br>
(4) "#Year2017 love life, and life will love you back"
<br>
(5) "RT @HillaryClinton: ‰ÛÏWay too many dreams die in the parking lots of banks. In America, if you can dream it, you should be able to do it.‰Û ‰ÛÓ‰Û_"
<br>
(6) "studying the humanities is necessary - we need both stem and humanities to be strong thinkers in 21st c. #highered http://t.co/64gyoZBCMR"
<br>

3 of the these are retweets, and 3 of them are tweets.

With all 2,529 datapoints, I have some questions: 

<br>
(1) how many of the tweets are retweets? 
<br>
(2) what are patterns in twitter behavior over time? 
<br>
(3) is my next tweet going to have anything to do with #DataScience?
<br>
(4) how is a supervised classifier able to classify tweets into tweets or retweets based on the text in them? 
<br>

These are all questions I'd like to answer over the next few weeks.

<br>


### Where are the metro stations? (written on 12/16/2017)
With [Compass](http://compassprobono.org), I'm working on another strategic alignment project to support an adjustment in [Homeless Children's Playtime Project's](https://www.playtimeproject.org) services, operations, and locations, as they move to new sites. One way I'm supporting the project is by collecting and analyzing data in a way that informs the organiation as the nonprofit make adjustments. 

Today,to support Homeless Children's Playtime Project, I started collecting data on the locations of homeless shelters, homeless services, metro stations, and bus stations. Most of the data I was collecting comes from [DC Open Data](http://opendata.dc.gov) but metro data came from [Ben Balter's dc-maps git repo](https://github.com/benbalter/dc-maps), so instead of just downloading the file with Lat and Lon, I enjoyed working on manipulating some of the data.

After saving the json file linked to the maps of [metro station entrances](https://github.com/benbalter/dc-maps/blob/master/maps/metro-station-entrances-district.geojson), I read the data and parsed out the Station Name, the Line, the Latitude, and the Longitude. I then save the parsed out data in a dataframe and read that data file out. There are similar blogposts on this topic that explore reading json files in more depth [here](http://zevross.com/blog/2015/02/12/using-r-to-download-and-parse-json-an-example-using-data-from-an-open-data-portal/).

<img class="picture" src="where-are-the-metro-stations-code.jpg">

Now our team has [data](https://github.com/margaretmf/DCMetros) to answer the question, "where are the DC metro stations?".

<br>
