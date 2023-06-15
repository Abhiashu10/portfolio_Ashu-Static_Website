---
title: "AirBnb Price Prediction- Explainable AI (LIME and SHAP)"
description: "Model Interpretation, Predict the price for listings using listing descriptions and features that affected the price"
dateString: Dec 2021
draft: false
tags: ["Explainable AI", "LIME", "SHAP", "Machine Learning"]
showToc: false
weight: 202
cover:
    image: "projects/Airbnb/Front.png"
--- 
### 🔗 [GitHub repository](https://github.com/Abhiashu10/Airbnb-Price-Prediction-LIME-and-SHAP/tree/main)

## Description
We use the Inside Airbnb dataset to identify significant trends in customer interest and predict the pricing of rentals in the US and Europe. This problem is similar to a classical use case of machine learning: house price prediction. We can then provide solutions to business difficulties.
We have used LIME and SHAP to interpret the model's predictions at the local and global levels. 

## Model Interpretation
1. Linear Regression: - We use LIME and SHAP to interpret the model's predictions at the local and global levels. We take a random test vector from the test set and set the number of the top features as 5, the number of perturbed samples as 5000.
![my notes](/projects/Airbnb/LI1.png)

The comparatively higher market value of the house reflected by the provided vector (depicted by a bar on the left) can be related to the following reasons: 
- The high value of room_type_private_room on the negative side indicates that because it’s a private room, the price will reduce.
- The high value of longitude on the negative side indicates that the house is not in a suitable place such as city centers or crowded neighborhoods.
- The high value of bedrooms on the positive side indicates that the house has a bedroom, which is a private room and people prefer it.
- The high value of review_scores_rating on the positive side indicates that the house has a high rating.
![my notes](/projects/Airbnb/LI2.png)
- At the global level, we can see that longitude, bedrooms, accommodates, latitude, beds, review_scores_rating affect the price most.

2. Decision Tree Regression: - At the global level, we can see that longitude, accommodates, latitude, bedrooms affect the price most.
![my notes](/projects/Airbnb/DT.png)

3. Random Forest Regression: - At the global level, we can see that longitude, accommodates, latitude, bedrooms affect the price most.
![my notes](/projects/Airbnb/RF.png)

4. XG BOost: - At the global level, we can see that bedrooms, room_type_entire_home/apt, accommodates, longitude, latitude affect the price most.
![my notes](/projects/Airbnb/XG.png)

##Code
## [GitHub Code](https://github.com/Abhiashu10/Airbnb-Price-Prediction-LIME-and-SHAP/blob/c92a3bf3c0d649030f38cb338d09dce4ce519798/Airbnb%20Price%20Prediction-Explainable%20AI.ipynb)

