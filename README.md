# Expoplanet-Hunting-in-Deep-Space 
The dataset for this project was found on [Kaggle](https://www.kaggle.com/keplersmachines/kepler-labelled-time-series-data)

![Outer Space](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/Images/outer%20space.png)

## What is an Exoplanet?
An Exoplanet is a planet which is not a part of out solar system. A Planet which might be a part of other star system (which would resemble to our solar system) could be called an exoplanet. Search for these exoplanets have been going on for decades in the hopes of finding an Earth-like planet which might be habitble to living organisms or hopefully Aliens.

![Kepler Exoplanet](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/Images/exoplanet.jpg)

## How exoplanets are detected? 
An exoplanet has to be orbiting a star, that is one of the consideration for being a planet. So as the exoplanet is orbiting a star, there are flux intensities (the light intensities) which can be measured. Planets themselves does not emit light but the star they oribiting doe. As the planet revolves around the star, the flux intensities changes with respect to time. Ocassional dimming can be seen over a period of months and years while observing it. This can imply that there exist an exoplanet and it is oribiting a star in a far far star system perhaps. This planet can then be considered a candidate and can go under inspection to be further confirmed.  

## Motivation behind this project 
I've always been fascinated by outer space and I stumbled upon the this dataset. Now, if I get a chance of detecting an exoplanet far far away in another Star system, I wouldn't have let it gone. 

## Flux intensity visualized 
There are 2 labels:
- Label 1 is a Non_exoplanet Star
- Lable 2 is a Exoplanet star

### Label 1 (Non-exoplanet star)
The below image shows the flux intensity of a non-exoplanet star randomly selected from the dataset

![Non-exoplanet Flux intensity](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/Images/Label%201.png)

### Label 2 (Exoplanet star)
The below image shows the flux intensity of a exoplanet star randomly selected from the dataset

![Exoplanet Flux intensity](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/Images/Label%202.png)

## Project 
The project was done firstly using Machine Learning algorithms. It is a classification project and I tried different machine learning classification models. For example, Logistics Regression, SVC, K-means, etc. The dataset here is extremely imbalanced. It was hence difficult for machine learning models to be great at predicting. The jupyter notebook can be found [here](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/exploplanet_hunting.ipynb). As I went further in my learning journey and learnt about Neural networks, I created models which was far better than the earlier machine learning models which I made. I used Convolution Neural Networks in 1D with tensorflow for creating a neural network model. The neural net jupyter notebook can be found [here](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/exoplanet_hunting_with_neural_nets.ipynb).

### Dataset
The training set here consisted of **37 exoplanets** and **5050 non-exoplanets**. 
On the other hand, the test set consisted of only **5 exoplanets** while there were **565 non-exoplanets**.
As you can see the ratio is very imbalanced. 

### Evaluation Metrics
As the dataset is highly imbalanced, the Evaluation metrics can behave uncannily under this circumstance. The evaluation metrics for classification model like `classification_report()` fails here. As the metrics, which we evaluate on, is immensely important for the balanced data, it is not quite good for the imbalanced data. Here the model can give you `1.0` result but, it actually detects correctly all the majority of the category in the imbalanced dataset.

The alternative which can be used here is, evaluating the model based on the Confusion matrix. The True Posivites, True Negative, False Positives and False Negtives can actually give us great result. Here you can see, just looking at the confusion metrics, we can clearly justify out of 5 exoplanets, 4 has been detected. 

![Confusion Metrics](https://github.com/VishalxRana/Expoplanet-Hunting-in-Deep-Space/blob/master/Images/Confusion%20matrix.png)

Label 1 is converted to label 0 and label 2 is converted to label 1.

Label 1 -> Label 0

Label 2 -> Label 1

# Conclusion 
It can be concluded that the model can predict 5 out of 4 exoplanets correctly. As the data is imbalaced, there needs to be more data especially of label 2 (Exoplanet Star), so that the model can correctly learn the patterns.  