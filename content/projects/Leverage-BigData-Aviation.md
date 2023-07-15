---
title: "Leveraging Big Data Analytics in Aviation Industry"
description: "Apache Spark as our big data analytics tool within the Hadoop ecosystem"
dateString: June 2022
draft: false
tags: ["Python", "PySpark", "Apache Spark", "EDA", "Big Data"]
showToc: false
weight: 205
cover:
    image: "projects/BigData/CoverBig.png"
--- 
### 🔗 [Github repository](https://github.com/Abhiashu10/BigData-PySpark-Project)

### 🔗 [Dataset Source](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/HG7NV7)

## Description
In this project, I have used the big data analytics tool, and performed an analysis on the metadata of the airline flights that occurred in the United States between the years 1987 and 2008. To begin, it is necessary for us to investigate the past of aviation in the United States.We chose **Apache Spark** as our big data analytics tool within the Hadoop ecosystem because spark is an open-source framework designed for ease of use, speed, and sophisticated analytics. In order to conduct our analysis, we relied on **PySpark**, which is essentially just the Python interface to Apache Spark.
Research Questions: -
- Which airline has the greatest amount of cancelled flights? Why do these Airlines have the highest amount of cancellations, and what can those causes be?
- Which year appears to have had the most flights cancelled overall, and  what may the potential causes be? Is it wise to make decisions only based on data?
- Which domestic airline routes in the US had the largest flight traffic, and between which two stations?
- Which airline is the world's biggest public airline companies by number of passengers carried between 1987 and 2008?
- Which airlines are the main rivals of the largest publicly traded airline corporations in the world in terms of passenger volume?
- Which year sees the most flight bookings and the aviation industry's boom?
- Which month of the year do individuals most frequently travel?
- Which day of the month saw the highest number of passengers taking flights?
- Which day of the week saw the highest number of passengers taking flights

## Methods and Key Findings

- Method 
we need to start a spark session in order to make effective use of the spark framework and API in this project, we imported a function called SparkSession from the PySpark library and then started a spark session. And below you will find the code that we executed in order to create a sparksession.
![my notes](/projects/BigData/B0.png)

- Key Findings

1. 
![my notes](/projects/BigData/B1.png)

2. 
![my notes](/projects/BigData/B4.png)

3. 
![my notes](/projects/BigData/B3.png)

4. 
![my notes](/projects/BigData/B4.png)


## Code

### 🔗 [Code](https://github.com/Abhiashu10/BigData-PySpark-Project/blob/08991cbdb8c3c8d4a06c6ba575059e9eafe72b3d/bigdata.ipynb)

