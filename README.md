# Customer-Segmentation
###### by Ibrahim Patel




![Alt Text](https://media.giphy.com/media/8JQ4e2E6s1DM8GLTKw/giphy.gif)
## Executive Summary
Consumerism is one of the main reasons businesses thrive so well today. If a business wants to improve its metrics of success one thing they must do is look into their customer base. We want to find interesting patterns and see how we can cluster the mall's customers into different groups. We will be using the K-Means Algorithm for Clustering. 

## Contents
1. [Introduction](#introduction)
    - [Problem Statement](#problem_statement)
    - [Dataset](#dataset)
2. [Analysis](#analysis)
    - [Data Cleaning](#data_cleaning)
    - [Exploratory Analysis](#exploratory_analysis)
    - [Modeling](#modeling)
    - [Results](#results)

## Introduction <a name="introduction"></a>


<p></p>

<p></p>

### Problem Statement <a name="problem_statement"></a>
Many different types of customers leisurely walk through the mall. Looking at different products ranging from hair, clothes, skin, toys, etc. Some customer will spend hours in the mall, and yet to make a purchase. While others may have barely step foot in the mall, but they are already swiping their credit card to make a purchase. Of course, these are two extreme ends of the spectrum, but it is our goal to group similar customers together. This will be done with K-means Clustering. 

### Dataset <a name="dataset"></a>
Here is a link to the dataset :
https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python

This is a dataset that I found on Kaggle.com. I will try to use an unsupervised learning approach to break up the customer population into different clusters. I will be using the K-Means Algorithm for Clustering. This is also my first attempt at making an Unsupervised Learning Model. Wish me luck!

Ps. The one con about this dataset set is that it only contains 200 observations making it a smaller dataset. However, I still think this is an amazing dataset that can be used for many different machine learning projects.



## Analysis <a name="analysis"></a>

### Data Cleaning <a name="data_cleaning"></a>

Thankfully this dataset did not contain any null values. Overall this dataset was clean from the start which is a good thing for us. 

### Exploratory Analysis <a name="exploratory_analysis"></a>

Here is a distribution of the "Spending Score". The "Spending Score" is a score given to customers depending on how often they shop, how much they buy etc. From this distribution, we can see that it has fat tails. Fat tails also imply a strong influence of extreme observations on expected future risk.  
 
<img width="686" alt="Screen Shot 2020-08-31 at 9 59 39 PM" src="https://user-images.githubusercontent.com/52756457/91789947-4bc53c00-ebd5-11ea-9e58-e1f531bc7efa.png">

Here is a distribution of the "Annual Income" of the different people in the dataset. We can see that it is skewed to the right. This makes sense because this distribution is saying that the majority of people make less than 80K a year while a much smaller percentage makes more than 80K a year. This gives us an idea of the demographic shopping. Overall this gives us a  good idea for moving forward with this project. 

<img width="669" alt="Screen Shot 2020-08-31 at 9 16 22 PM" src="https://user-images.githubusercontent.com/52756457/91788382-aa88b680-ebd1-11ea-860a-351b59a57f4a.png">

Here we can see the distribution of "Annual Income" for both genders. We can see that there are more females than males with an income of 60-80k.

<img width="727" alt="Screen Shot 2020-08-31 at 9 16 45 PM" src="https://user-images.githubusercontent.com/52756457/91788946-1d466180-ebd3-11ea-98d0-ac12367a12ef.png">





### Modeling <a name="modeling"></a>
I took an unsupervised learning approach when doing this problem. I used the K-Means Clustering algorithm because it is used to find groups that have not been explicitly labeled in the data. This can be used to confirm business assumptions about what types of groups exist or to identify unknown groups in data sets. 

![Alt Text](https://media.giphy.com/media/loMkMSW589EA2LKxQX/giphy.gif)



### Results <a name="results"></a>

<img width="520" alt="Screen Shot 2020-08-31 at 8 00 41 PM" src="https://user-images.githubusercontent.com/52756457/91789039-5a125880-ebd3-11ea-9106-4e5a3c7c8c1b.png">

We can see by looking at the scree plot that there is not much change in the number of distortion as the number of clusters increases past 12. This is saying that after making 12 different groups there is a lot less error happening than if we had fewer groups. Also, the flattening line is telling us that adding more clusters won't do much in lessening the distortions.

<img width="557" alt="Screen Shot 2020-08-31 at 8 00 08 PM" src="https://user-images.githubusercontent.com/52756457/91789092-7dd59e80-ebd3-11ea-9722-e215358b126a.png">

By looking at the silhouette plot we can see the dotted red line is out silhouette score. A silhouette score ranges from -1 to 1. The silhouette score represents how similar an object is to its own cluster (cohesion) compared to other clusters (separation). We got a silhouette score of roughly .4 which is not bad for our first attempt at making an unsupervised learning model. 

To view the full extent of my work you are more than welcome to browse through the notebook. To get a better understanding of my findings to feel free to read my blog at 
https://www.ibbysblog.com/. 

I will work on this project in the future, and try my best to make my model better by doing more feature engineering.


