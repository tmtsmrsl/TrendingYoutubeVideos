# TrendingYoutubeVideos  
An analysis on a list of ~47k trending videos appearances in Indonesia since the beginning of this year up to 13 Sep 2022 (around 200 trending videos were updated on each day). You can visit my project [here](https://deepnote.com/@tmtsmrsl/Trending-Youtube-Videos-in-Indonesia-2022-2b996b1b-6a67-4baa-966c-7e2d0a6610f2). Throughout the analysis I managed to solve the following questions:  
* What are the most and least popular video categories in 2022?  
* When is the optimal day/time to publish youtube videos?  
* Which videos and channels appear the most on the trending page?  
* What are the most popular keywords for titles and tags?  
* How do video definition and caption availability affect the chance of a video becoming trending?  
* How often do videos in other languages (besides Indonesian) appear on the trending page?  
* How does the engagement rate (like and comment count per view) differ between categories?  
* Etc.  

The project is done using Python and include the following steps. First I made an ETL pipeline to request the data from Youtube API, transform it from json format to dataframe, and load the data into BigQuery table. Since it's not possible to request trending videos data in the past, I resorted to using a [dataset](https://www.kaggle.com/datasets/syahrulhamdani/indonesias-trending-youtube-video-statistics) which is updated daily by Syahrul B Hamdani. Then I performed data wrangling to remove unnecessary data, convert the data type and handle missing value. And last I did the EDA along with the visualization, which involves image manipulation with PIL, requesting additional data (youtube channel infos and videos language) from Youtube API, making waffle chart using a scatter plot and a bit of NLP technique. If you are interested with the code, you can visit my notebook [here](https://deepnote.com/workspace/datascience-d6c9-c207135c-4160-4f0c-81dc-c822e8fdd43e/project/Trending-Youtube-Videos-in-Indonesia-2022-2b996b1b-6a67-4baa-966c-7e2d0a6610f2/notebook/Trending_Youtube_Videos-5e6d070a6c5e4f59a1d9e91b71564559#1633f18521014fcb8aa589221e395c29)
