---
layout: page

---
 
![title]({{site.url}}/images/predict.png)

## Project Overview and objectives: 

Is about scraping a website to acquire data, subsequent building a linear regression model to make predictions.
### objectives: 
+ Scrape a Times Higher Education Website using python and Selenium library.
+ Analyze the nature of the obtained data to summarize their main characteristics.
+ Train and validate various models and pick the best fit model.
+ Test and validate the selected model.

## Motivation:
The cost of a degree is an important determinant of the decision to apply to an university.Everyone should have the same opportunity to attend college without being in debt. Each year the tuition either increases or slightly decreases, based on certain measurements.


## Workflow:

![flow]({{site.url}}/images/flow.png)

### Step 1 : Web Scraping
In this step, Selenium used to extract data from Times Higher Education. Scraped three tables which are: World University Rankings, US  College Rankings, and Japan University Rankings. Some Features:
+ Citations
+ Engagement
+ Environment
+ International Students
+ International Outlook
+ Research
+ Resources
+ Teaching
+ Tuitions and fees
+ Industry income

### Step 2 :Data processing and Exploratory Data Analysis (EDA)

In this step, the tuition fees in the Japanese universities table is converted from yen to dollars. The reason why the World Universities table was scrapped is to merge the US and Japanese universities with International indicators.

### EDA :
 For students wondering why study in Japan, tuition fees can be a major deciding factor. Especially in comparison to the US, tuition fees in Japan are comparatively cheap.
The figure below shows 
![US_Japan_cluster]({{site.url}}/images/US_JAP.png)

In the US, "in-state" students generally pay at least $10,000 a year on tuition.
Besides ,Japanese students generally pay at least $5300 a year on tuition.


### Distribution of Tuition :  

![distribution]({{site.url}}/images/distributions.png)


### Heat Map:  
The heat map shows a  high correlation between Citations , International Students and International Outlook with Tuition
![heatmap]({{site.url}}/images/cor.png)

### Pair Plot:
pair plot shows that the Tuition has an almost linear relationship with Citations, International Students, International Outlook, Research and Teaching which indicates that it is a great value to any model that we are going to create.

![pairplot]({{site.url}}/images/pairplot.png)


### Step 3 : Models Building and Selection
In this stage, a set of models were built. Some models included some of  variable transformations. Moreover, should be mentioned that any feature has a p-value > 0.05 was excluded from the model.

![models]({{site.url}}/images/models.png)


### Plots for the Best Model :

![plot.png]({{site.url}}/images/plot.png)

### Actual vs Predicted Values


![act_pre]({{site.url}}/images/act_pre.png =120x240)


