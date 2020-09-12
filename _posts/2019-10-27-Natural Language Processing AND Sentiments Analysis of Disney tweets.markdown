---
layout: post
title: "Natural Language Processing AND Sentiments Analysis of Disney tweets"
date: 2019-10-27

img: giphy_ds.gif # Add image post (optional)
---



## Project Overview and objectives: 

The Walt Disney Company is a productive powerhouse of a multinational corporation, As with most businesses that they have a vested curiosity in estimating how their customers and the public feeling about their services that they provide and the products that they produce, but obtaining that information, whether through in-person, over the phone, or surveys, cost money and time to create, distribute, gather, and analyze. Therefore, I am interested in observing if I use Natural Language Processing (NLP) tools and unsupervised machine learning to assess public opinion of Disney at a minimal cost.


![flow](https://media.giphy.com/media/k4ZItrTKDPnSU/giphy.gif){:width="900px"}


### Data acquisition

First, I wanted data in the form of text, which is publicly posted; hence I turned to Twitter. I was using the Twitter API (Application Program Interface), which takes less than 24 hours to get approval. Next, Fetched  50,000 tweets related to the keyword and hashtag #Disney in English for a week.

### Data cleaning :
![cleaning](https://media.giphy.com/media/YRLFCiISitFEQ/giphy.gif)

+ Remove URLs , Stop-words , Punctuations , Numbers

+ Convert text to lower-case 

+ Convert  emojis to words

+ Lemmatization

### Words Counts 

![distribution]({{site.url}}/assets/img/mickeycount.png )


### Vectorize & Dimensionality Reduction


I have tried a bunch of techniques to reduce the dimensionality like Latent Semantic Analysis (LSA), Biterm, and Non-negative Matrix Factorization (NMF). However, I determined that NMF with a count vectorizer works more suitable for the data regarding the short length and lack of context.

![tf]({{site.url}}/assets/img/tfdis.png)


### Sentiments Analysis :
 IT IS DISNEY !!  ALL POSITIVES ! :)


![models]({{site.url}}/assets/img/SEN_DIS.PNG)

