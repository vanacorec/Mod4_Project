# Mod4_Project

# Image Classification of Dogs and Cats by Breed

## Motivation
We wanted to see if we could predict a dog or a cat by breed just from a photo. Our goal was to create a model that we could input an image to predict the breed of dog or cat.  

## Sources
We took .png files of images of dogs and cats from the Oxford-IIIT Pet Dataset (http://www.robots.ox.ac.uk/~vgg/data/pets/). We also suplemented this data with the Stanford Dog Dataset (http://vision.stanford.edu/aditya86/ImageNetDogs/) and added the breeds that they had incommon together and just kept the 37 different breeds from the Oxford dataset.  However the majority of our analysis was just done on the Oxford-IIIT Pet Dataset.

## Exploratory Data Analysis 
This shows the amount of picture by breed in the Oxford dataset: 

![image of spreadsheet](/readme/OxfordPetData.png)

## Data Organization 
After EDA, we split the data into folders by breed and then split that into train and test data.

## Best Model Results
Our best performing model had a tvalidation accuracy and a test accuracy score of 88%. We used transfer learning and stacked two CNN models on top of each other (VGG19 and Resnet50). However this model took a long time to run and would crash colabs from using too much RAM.

![image of best model outcomes](/readme/BestModel.png)

## Model Results
Given the computing power problems we actually perfer our second best model as it has a validation accuracy score of 83%, only took 10 minitues to run and doesn't crash Colabs. This model uses InceptionV# with weights as the base model.

![image of next model outcomes](/readme/imagenet2_testcm.png)

![image of next model outcomes per epoch](/readme/validation.png)

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
