---
layout: post
title: "Find IT!-The Cheapest Alternative"
date: 2019-11-20

img: p5_tot.png 

---



## Project Overview 

Following up with the fashion trend is still the major theme that runs the retail fashion business. Also, As a person who enjoys fashion, I know that inspiration can come from various sources when it comes to obtaining a great outfit. Perhaps you got inspired by someone you follow on the social media "a fashionista " or by a celebrity.  Concerning most consumers, shopping for stylish and affordable outfits is a never-ending quest. Usually, the Trends styles, designed by the high-end brands designer, they are too expensive for regular consumers. 
However, it is hard and consuming for shoppers to find a cheap alternative to a target style as long as shoppers should determine the outfit that suits what they need over several websites and then obtain the cheapest from the matched outfits. 
My project aims to recommend the more affordable alternatives to a designer outfit by using convolutional neural networks and other techniques.



### 1.Data acquisition:

![flow]({{site.url}}/assets/img/Myntra-online-shopping.jpg)

I Got the data set from my nrta .com is an Indian website  , contains 44447 images with their json files , from all departments , and 51  Categories.


### 2.Date preprocessing 

+ Extract features for each image from the json file .
+ Convert Indian Rupee to Dollars $  .
+ Limited to just 250$ and under.
+ Just keep clothing departments images with 16 categories .
+ Image Augmentations  for categories balance .
+ Resize and normalize all the images to the same size.





### 3.Model:
The project is comprised of two main parts:

1. Classify the category of the clothing in an input image

2. Retrieve a similar and cheaper outfit.


### 3.1 CNN :  
In this step, I used a convolutional neural network (CNN) to predict the clothing category.
The model was trained with the training dataset for three convolutions layers, two dense layers, dropout of 0.5 .

![cnn_model]({{site.url}}/assets/img/cnn_model.png){:height="600px" width="500px"}

The Accuracy: 89%

![cnn_model]({{site.url}}/assets/img/p5_trainacc.png)

### 3.2 Recommendations:
After the classification, I extract the output of the second fully connected layer as features.
Converted images into a feature matrix to calculate the cosine similarity, then selected the top 3 images with the largest cosine as the recommendations. And calculate the  Euclidian similarity, then selected the top 3 images with the smallest Euclidian similarities as the recommendations.

#### 3.2.1 Demo


![sarees]({{site.url}}/assets/img/sarees.png){:height="500px" width="550px"}


![sarees]({{site.url}}/assets/img/sarees_price.png){:height="500px" width="550px"}


I picked a Saree from Kalki Fashion website that cost 290 $

<video width="800" height="740" controls>
  <source src="/assets/img/sareedemo.mov" type="video/mp4">
</video>




What I remarked when using the cosine and euclidian similarities for the same input image that the cosine recommends a better match with the cut/style, whether the euclidian recommends better match colors.

![same_input.png]({{site.url}}/assets/img/same_input.png)





