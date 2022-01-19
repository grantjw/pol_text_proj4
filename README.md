# Hiliary Clinton Email Text Analysis: Overview 
* Analyzed Hilary Clinton’s 8000 emails with Principal Components Analysis, Structural Topic Modeling, and Sentiment Analysis using R.
* Identified 3 clusters of emails to reveal politically sensitive issues related to Hillary Clinton such as discussions on Benghazi.
* Full code is uploaded as an html file and R Markdown file. The full writeup is uploaded as a pdf file. 

## Executive Summary
We start with exploratory analysis on the entire trigram dataset using the Principal Components Analysis resulted in two general findings: 
* First, there are subsets of emails that form unique clusters. 
* Second, the variables “house_select_benghazi,” "re_turkey_armenia," "Huma Abedin" account for substantial variation in the entire dataset. 

We further delve into the data by conducting STM with 27 topics and do a sentiment analysis on these topics: 
* found that some topics did not match our preconvieced notions given the US relationship with certain countries
* topics 5, 14 and 18 correspond to the three variables identified in the PCA analysis on the entire dataset. 

In turn, we do PCA analysis for each topic 5, 14, and 18. There are three findings: 
* First, there are identifiable clusters of emails that discuss the "Turkey-Armenia'' relationship with former prime minister of Turkey Ahmet Davutoglu involved. 
* Second, emails about Lona Valmoro and Huma Abedin can be sub-categorized and viewed separately. 
* Lastly, not only the words “redactions", "benghazi", "sensitive" are closely related but also they serve to cluster some of the emails that were also identifiable as clusters in the entire PCA analysis, meaning that they are distinct from other emails and must be further studied.

## Dataset
Text data set pertaining to approximately 8000 emails that were sent and received on Hillary Clinton's private accounts. These data were released by the U.S. State Department in 2015.
The stucture of the dataset is as follows: 
* Each row represents a unique email.
* Columns 1 to 9 contain metadata.
* Columns 10 to 3009 contain counts of the top 3000 frequent unigrams.
* Columns 3010 to 4009 contain counts of the top 1000 frequent bigrams.
* Columns 4010 to 4509 contain counts of the top 500 frequent trigrams.

Further details about the data can be found [here](https://www.kaggle.com/kaggle/hillary-clinton-emails) 


