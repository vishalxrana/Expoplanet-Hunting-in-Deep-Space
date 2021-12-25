# Expoplanet-Hunting-in-Deep-Space 
The dataset for this project was found on [Kaggle](https://www.kaggle.com/keplersmachines/kepler-labelled-time-series-data)

## What is an Exoplanet?
An Exoplanet is a planet which is not a part of out solar system. A Planet which might be a part of other star system (which would resemble to our solar system) could be called an exoplanet. Search for these exoplanets have been going on for decades in the hopes of finding an Earth-like planet which might be habitble to living organisms or hopefully Aliens.

## How exoplanets are detected? 
An exoplanet has to be orbiting a star, that is one of the consideration for being a planet. So as the exoplanet is orbiting a star, there are flux intensities (the light intensities) which can be measured. Planets themselves does not emit light but the star they oribiting doe. As the planet revolves around the star, the flux intensities changes with respect to time. Ocassional dimming can be seen over a period of months and years while observing it. This can imply that there exist an exoplanet and it is oribiting a star in a far far star system perhaps. This planet can then be considered a candidate and can go under inspection to be further confirmed.  

## Motivation behind this project 
I've always been fascinated by outer space and I stumbled upon the this dataset. Now, if I get a chance of detecting an exoplanet far far away in another Star system, I wouldn't have let it gone. 

## Flux intensity visualized 
There are 2 labels:
- Label 1 is a Non_exoplanet Star
- Lable 2 is a Exoplanet star

### Label 1
This image is a random Label 1 flux intensity in a plot

### Label 2
This image is a random Label 2 flux intensity in a plot 

## Project 
The project was done firstly using Machine Learning algorithms. It is a classification project and I tried different machine learning classification models. The dataset is extremely imbalanced. The evaluation metrics for classification model like `classification_report()` fails here. As the metrics which we evaluate on is immensely important for the balanced data it is not quite good for the imbalanced data. Here the model can give you `1.0` result but, it actually detects correctly all the majority of the category in the imabalced dataset. 
The alternative which can be used here is, evaluating the model based on the confusion matrix. The True Posivites, True Negative, False Positives and False Negtives can actually give us great result. 
  