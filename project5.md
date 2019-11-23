---
layout: page

---

![title]({{site.url}}/images/p5_tot.png)

## Project Overview 

following up with the fashion trend is still the major theme that runs the retail fashion business. Also, As a person who enjoys fashion, I know that inspiration can come from various sources when it comes to obtaining a great outfit. Perhaps you got inspired by someone you follow on the social media "a fashionista " or by a celebrity.  Concerning most consumers, shopping for stylish and affordable outfits is a never-ending quest. Usually the Trends styles, designed by the high-end brands designer, they are too expensive for regular consumers. 
However, it is hard and consuming for shoppers to find a cheap alternative to a target style as long as shoppers should determine the outfit that suits what they need over several websites and then obtain the cheapest from the matched outfits. 
My project aims to recommend the more affordable alternatives to a designer outfit by using convolutional neural networks and other techniques.




### 1.Data acquisition:

![flow]({{site.url}}/images/Myntra-online-shopping.jpg)

I Got my data set from my nrta .com is an Indian website  , contains 44447 images with their json file , from all departments , and 51  Categories.


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
In this step,used convolutional neural network (CNN) to predict clothing category
The model was trained with the training dataset for 3 convolutions layers ,2 dense layers ,dropout of 0.5

![cnn_model.png]({{site.url}}/images/cnn_model.png =250x)

The Accuracy: 89%

![cnn_model.png]({{site.url}}/images/p5_trainacc.png)

### 3.2 Recommendations:
After the classification, I extract  the output of the second fully connected layer as features .
Converted images into a feature matrix. To calculate the cosine similarity, then, selected the top 3 images with the largest cosine as the recommendations. and calculate the  Euclidian similarity, then selected the top 3 images with the smallest Euclidian similarities as the recommendations.

#### 3.2.1 Demo
I picked a Saree from Kalki Fashion website that cost 290 $

![sarees.png]({{site.url}}/images/sarees.png)

#### 3.2.1 Demo
![Watch the video]({{site.url}}/images/sareedemo.mov)

![same_input.png]({{site.url}}/images/same_input.png)
What I remarked when using the cosine and euclidian similarities for the same input image that, the cosine recommends a better match with the cut/style, whether the euclidian recommends better match colors.



