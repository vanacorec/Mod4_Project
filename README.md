# Mod4_Project

# Image Classification of Dogs and Cats by Breed

## Motivation
We wanted to see if we could predict a dog or a cat by breed just from a photo. Our goal was to create a model that we could input an image to predict the breed of dog or cat.  

## Sources
We took .png files of images of dogs and cats from the Oxford-IIIT Pet Dataset (http://www.robots.ox.ac.uk/~vgg/data/pets/). We also suplemented this data with the Stanford Dog Dataset (http://vision.stanford.edu/aditya86/ImageNetDogs/) and added the breeds that they had incommon together and just kept the 37 different breeds from the Oxford dataset.  However the majority of our analysis was just done on the Oxford-IIIT Pet Dataset.

## Exploratory Data Analysis 
This shows the amount of picture by breed in the Oxford dataset: 

![image of spreadsheet](/Screen%20Shot%202019-03-29%20at%2011.23.03%20AM.png)

This graph shows ______________:

![image of graph of work counts per author](/Screen%20Shot%202019-03-29%20at%201.11.14%20PM.png)

This graph shows ________________: 

![image of graph of word counts per author](/Screen%20Shot%202019-03-29%20at%201.10.31%20PM.png)

## Data Organization 
After EDA, we split the data into folders by breed and then split that into train and test data.

## Data Analysis
Our best performing model had a testing accuracy score of ______. We used transfer learning and stacked two CNN models on top of each other (VGG19 and Resnet50).

![image of best model outcomes](/Screen%20Shot%202019-03-29%20at%201.12.01%20PM.png)

![image of AOC of best model](/Screen%20Shot%202019-03-29%20at%201.12.24%20PM.png)

## Model Results
We made multiple models with multiple parameters to get the best model possible. After multiple models and hyper parameter tuning we found that a transfer learning model with VGG19 and Resnet50 model worked best. Our model predicts with approximately ______% accuracy. Given that this is a multiclass classification model based on image data, this is wonderful. However, this model took a very long time to run, and crashed Colabs from too much RAM useage. Therefor we actually perfer our second best model as it has a validation accuracy score of 83%, only took 10 minitues to run and doesn't crash Colabs. 

## Frameworks / Libraries Used:
- Sklearn
- Matplotlib
- Pandas
- Numpy
- Itertools
- Scipy 
- Keras
- TensorFlow
- Random
- os
- shutil 
- re
- Pillow
- Scipy

## Credits
By Lois Rosenbloom and Caroline Vanacore
