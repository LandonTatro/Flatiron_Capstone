# An Analysis of Film Factors for Association with Profitability
Authors: Dima Taher, Leo Muntaner, Landon Tatro, Morgan Pelletier 
(Deloitte Strategy and Analytics - Orlando)

# GitHub Navigation Instructions 

Notebooks Folder

- For a detailed overview of our complete analysis, please reference the final notebook.
- To review our archived files, including exploratory data analysis files and individual analysis files, access the archived files folder.

Data Folder

- To review each of our datasets, access the data folder. 

# Overview

We conducted a series of analyses to determine associations between various facets of films and generated profit/revenue. Our results lead to the following suggestions for Computing Vision:

1. Aim to hire more experienced directors for profit security. 
2. Aim to release films on Fridays in order to maximize box office revenue
3. While we do not suggest using genre as a method of profit security, we do suggest additional research into potential confounding factors that may target higher median profit in animation, adventure, science fiction, action, and fantasy movies. 


# Business Understanding

## The Problem

We were tasked with providing Computing Vision a series of suggestions for their transition into the film industry. Specifically, we aimed to determine suggestions that could target higher levels of revenue and/or profit.

## The Goal

The film industry is a creative and diverse market with several avenues to success. With the understanding that there is no one path to success, we aimed to generate insight into a variety of actions Computing Vision may want to take in order to carve their own unique path to success. To accomplish this goal, we analyzed several different facets of films and their relation to generating revenue and profit. These areas included genres, day of release, and experience level of directors. 

# Data Understanding and Analysis

## Data Sources, Descriptions, Relevant Visualizations

The range of our analyses required utilization of several datasets. For each area of analysis, we used:

Directors:
 - Movie Info dataset, which is from Rotten Tomatoes which included the Director column required for this analysis with 1,560 rows.
 - Movie Budgets dataset from The-Numbers.com which included the movie titles, production budget, and worldwide gross revenue which we used to calculate the profit which is our main measure of success in the project, the columns had 5,782 rows.

Release Day:

Genres:
- Movie budgets dataset from the-numbers.com including movie titles, production budget, and worldwide gross revenue with 5,782 rows.
- TheMovieDB dataset including movie titles and genres with 26,517 rows.
- IMDB database: movie_basics table, which contains movie and genre information for approximately 140,000 entries.


# Methods 

## Programming Methods

Language: Python 3.1.1

Major Packages and Version Numbers can be found [here](requirements.txt)
    
## Data Science and Statistical Methods

By comparing distribution of profits by experience level of directors, we found a trend between increased experience and increased average profit. Specifically, after three movies, the distribution of profits was entirely positive. Because of this, we suggested that Computing Vision aim to hire directors who have directed at least three movies for profit security. 

By comparing median box office revenue by day of the week, we found that movies released on Thursdays had greater median box office revenue. This aligns with the observation that a large proportion of films are released on Fridays. This led us to suggest that Computing Vision aim to release their films on Thursdays in order to maximize box office revenue. 

We explored the relationship between genre and profit by comparing the distribution of profits for each genre. As a result, we found that animation, adventure, science fiction, action, and fantasy movies had greater variability. However, their median profits were much greater than that of other genres.

To further explore this avenue, we used a series of Chi-Square analyses (a method of comparing categorical data) coupled with the Cramer's V value (which determines the strength of any association) between Genre and profit level. The results were statistically significant, but the Cramer's V value was small and indicated a very weak association between the two variables. This implies that there is no evidence that Computing Vision should rely on genre as a source for profit security. However, future research into confounding factors that may explain the greater profit medians for genres such as animation and adventure would be beneficial. 


# Conclusions 

Based on our analyses, we suggest the following actions for Computing Vision:

1. Aim to hire more experienced directors for profit security. 
2. Release movies on Thursdays to maximize box office revenue.
3. While we do not suggest using genre as a method of profit security, we do suggest additional research into potential confounding factors that may target higher median profit in animation, adventure, science fiction, action, and fantasy movies. 
