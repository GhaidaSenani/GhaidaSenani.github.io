---
layout: page
title: Project 4
---

Natural Language Processing AND Sentiments Analysisof Disney tweets

 
![title]({{site.url}}/images/giphy_ds.gif)
## Project Overview and objectives: 

The Walt Disney Company is a productive powerhouse of a multinational corporation, As with most businesses that they have a vested curiosity in estimating how their customers and the public feeling about the services that they provide, and the products that they produce, but obtaining that information, whether through in-person, over the phone, or  surveys, cost money and time to create, distribute, gather, and analyze. Therefore, I am interested to observe if I use Natural Language Processing (NLP) tools and unsupervised machine learning to assess public opinion of Disney at a minimal cost.


![flow](https://media.giphy.com/media/k4ZItrTKDPnSU/giphy.gif | width=100)


### Data acquisition

First, I wanted data in the form of text, which is publicly posted, hence I turned to Twitter. Using the Twitter API (Application Program Interface) takes less than 24 hours to get the approval. I Fetched  50,000 tweets related to keyword and hashtag #Disney in English  
for one week.

### Data cleaning :
![cleaning](https://media.giphy.com/media/YRLFCiISitFEQ/giphy.gif)

+ Remove URLs , Stop-words , Punctuations , Numbers

+ Convert text to lower-case 

+ Convert  emojis to words

+ Lemmatization

### Words Counts 

![distribution]({{site.url}}/images/mickeycount.png )


### Vectorize & Dimensionality Reduction

I have tried a bunch of techniques to reduce the dimensionality like Latent Semantic Analysis (LSA), Biterm, and Non-negative Matrix Factorization (NMF). However, I determined that NMF with a count vectorizer works more suitable for the data regarding to the short length and lack of context.

![tf]({{site.url}}/images/tfdis.png)


### Sentiments Analysis :
 IT IS DISNEY !!  ALL POSITIVES ! :)


![models]({{site.url}}/images/SEN_DIS.PNG)

