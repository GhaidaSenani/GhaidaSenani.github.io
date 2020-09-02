---
layout: post
title: "WomenTechWomenYes EDA"
date: 2019-09-06

img: logo.png # Add image post (optional)
---

![logo]({{site.url}}/assets/img/logo.png)

## Problem Statement
WomenTechWomenYes (WTWY) will be hosts an annual gala at the beginning of the summer. They try to do double duty with the gala both to fill the event space with individuals passionate about increasing the participation of women in technology. So, they proposed us to discover the proper times, days and stations in New York subways, to place teams at stations to reach the maximum amount of people.

## Data Acquisition 

 MTA, NYC subways data for two months  May 'Before summer' , August 'Summer' 2019.	

## Data cleansing 

+ Removing white spaces in columns’ names.
+ Handling Entries and Exits accumulation process
+ Dealing with missing and negative values.

We have calculated the total traffic: Entries difference + Exits difference.

## Visuals
### Top five Stations based on Average traffic in May 
![MayTopAvgStations]({{site.url}}/assets/img/MayTopAvgStations.png)
### Top five Stations based on Average traffic in August 

![AvgTopFiveStation]({{site.url}}/assets/img/AvgTopFiveStation.png)
### Averrage Traffic Per hour During the weekdays
![Average_Traffic_wekdays]({{site.url}}/assets/img/Average_Traffic_wekdays.png)
### Averrage Traffic Per hour During the weekends
![Average_Traffic_weekends]({{site.url}}/assets/img/Average_Traffic_weekends.png)

#### We Recommend  A DEKALB AV station in August and A BAYCHESTER station in May  at 2-4 PM During Weekdays
#####  We obtained zeros in the total traffic in some Stations , So we considered  the situation of some  closed stations on certain dates on the month of August, due to some maintenance services

