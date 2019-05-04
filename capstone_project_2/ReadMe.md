# Capstone Project 2: Bungie Public Opinion Analysis

This is the repository for my second capstone project: Public Opinion Twitter Analysis for Bungie and Destiny 2, part of my <a href='https://www.springboard.com/workshops/data-science-career-track-course/'>
  SpringBoard Data Science Career Track Bootcamp
</a> curriculum.

## About this project

The purpose of this project is to analyze the engagement metrics and sentiments of tweets made about the company Bungie and their hit game Destiny 2. I will also attempt to correlate these metrics and sentiments with those of the tweets made by the official Bungie (@Bungie) and Destiny (@DestinyTheGame) Twitter accounts. The goal is to see if there are trends among what makes popular tweets about Destiny 2 or Bungie, and to see what people think about the company and the game.

I explored several trends among retweets, favorites, follower counts, posting times, and posting times since @Bungie or @DestinyTheGame tweeted. 

I used an excellent sentiment analysis package called
<a href='https://github.com/cjhutto/vaderSentiment'>
  VADER
</a>
to explore the connotations of the tweets, finding where it was accurate and where it fell through. Notably, most text about fighting is assigned negative connotation, but Destiny 2 is a shooter game, so fighting is the point.

Machine learning regressions trying to predict the exact number of retweets did very poorly, but assigning the retweet numbers to categories (< 100, < 10000, or >= 10000) and using classifiers performed excellently! From this, I discovered that the sentiment of a tweet is almost as important as the follower base of the posting user. Even further, positive tweets are much more likely to be spread than negative tweets, indicating that the community around Bungie and Destiny 2 looks at them fondly.

## About this repository

This repository contains the data files and the Jupyter notebooks for each of the steps in my project's analysis.

The documentation is in the following
<a href='https://drive.google.com/drive/folders/1_DH7jWmtUbsXEn3nO4kUtrzr54isCP0P?usp=sharing'>
  Google Drive folder
</a>.

<a href='https://docs.google.com/document/d/1UwVEpFjcgC2fUcAw37QPbU8hVG6iyC2QOmcPCQZJb48/edit?usp=sharing'>
  Original Project Proposals 
</a>
<br>
<a href='https://docs.google.com/document/d/1N9RLg7MNZEp9dXRO0IY2DsX3aF7VKjsrUi38YlHKgU0/edit?usp=sharing'>
  Final Project Proposal
</a>

### Capstone Project Process
The process for this capstone project is as follows:

Data is acquired and exported to csv in the data wrangling 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_2/notebooks/twitter_api_data_wrangling.ipynb'>
  notebook
</a>.

Data is visualized and explained in the data storytelling 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_2/notebooks/twitter_project_data_storytelling.ipynb'>
  notebook
</a>.

Data is analyzed statistically in the exploratory data analysis (EDA) 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_2/notebooks/twitter_project_eda.ipynb'>
  notebook
</a>.

Data is analyzed with machine learning in the in-depth analysis (IDA)
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_2/notebooks/twitter_project_ida.ipynb'>
  notebook
</a>.

<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_2/reports/capstone_project_2_final_report.pdf'>
  Final report
</a>
<br>
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_2/reports/capstone_project_2_presentation.pdf'>
  Final Presentation
</a>
