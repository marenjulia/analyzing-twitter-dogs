# Analyzing Twitter Dogs
This project was created for Udacity's Data Analyst Nanodegree. It used an enhanced Twitter archive of the account @dog_rates (WeRateDogs), a related image prediction file and additional Twitter API data to practice Data Wrangling skills and create meaningful analyses.

## Table of Contents
1. [Installations](#installations)
2. [Project Motivation](#motivation)
3. [File Overview](#overview)
4. [Key Results](#results)

## <a id="installations"/> Installations

This project used Python 3 within Jupyter Notebook, plus the following libraries: 
- pandas
- NumPy
- requests
- os
- json
- tweepy
- matplotlib and seaborn
- time
- PIL
- io

## <a id="motivation"/> Project Motivation

The motivation of this project was to practice data wrangling skills by:
- Gathering data about WeRateDogs tweets from three different sources (manual gathering, programmatic gathering using requests, programmatic gathering using Python's Twitter API tweepy)
- Assessing the data for data quality and data tidiness issues, with a special focus on the dog ratings
- Cleaning the data, using a _Define - Code - Test_ process to address the issues identified in the assessment stage
- Creating meaningful analyses based on the cleaned master dataset

The questions posed during analysis were: 
1. What is the average dog rating? Has the average rating changed over time?
2. Which dog breed is most popular?
3. Is there a relationship between number of retweets, number of favorites and ratings?

##  <a id="overview"/> File Overview
- wrangle_act.ipynb: Code for Data Wrangling, including gathering, visual and programmatic assessment, cleaning, and analysis and visualization
- wrangle_report.pdf: Report detailing wrangling efforts, e.g. listing identified data quality and tidiness issues and methods they were assessed with
- act_report.pdf: A blog-like report communicating insights and visualizations produced from the wrangled data
- data: 
  - twitter_archive_enhanced.tsv: @dog_rates Twitter archive, enhanced by Udacity
  - image_predictions.tsv: output of a neural network classifying Twitter images into dog breeds
  - tweet_json.text: data retrieved from Twitter API
  - twitter_api_data.csv: data retrieved from Twitter API (stored in csv for assessment)
  - twitter_archive_master.csv: end product of wrangling phase

## <a id="results"/> Key Results 

WeRateDogs' average rating is a 10.6/10. 75% of all ratings are at 10/10 or higher. The average rating for tweets rating dogs (as per the image prediction) is 10.9/10, the average non-dog rating at 9.5/10. The average rating has increased over time, from 10/10 in the beginning of 2016 to 12.8 in July 2017.

The dog breed that is most tweeted about, and has the highest aggregated favorite count and retweet count is the Golden Retriever. The highest rated dog breed, with on average 14/10, is a Gordon Setter. The most retweeted and favorited tweet shows a pupper kissing a French Bulldog.

Ratings are not correlated to favorite counts and retweet counts. Favorite count and retweet count have a strong positive correlation.
