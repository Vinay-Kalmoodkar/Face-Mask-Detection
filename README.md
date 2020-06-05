# Face-Mask-Detection

## Problem Statement
To detect whether or not a person is wearing a face-mask by using **Convolution Neural Networks** and **OpenCV**

## Dataset 
This dataset contains a `data` folder which contains 2 subdirectories namely
1. `without_mask` - which contains 686 images without mask.
2. `with mask`- which contains  690 images with masks.

The original dataset is prepared by [Prajna Bhandary](https://www.linkedin.com/in/prajna-bhandary-0b03a416a/) and available at [Github](https://github.com/prajnasb/observations/tree/master/experiements/data)

## Image Preprocessing
All the images are not of the same size, and neural networks often expect images that are standardized; a fixed size.
Therefore, the following preprocessing steps are performed:
* Gray scaling 
* Normalize
* Resize 
* Reshape

## Model Building and Training :
* Here a basic model is built using CNN and Keras library.
* Model is first trained on both **with and without masks images**.
* Then model is tested on sample test data. Whichever model is giving the good accuracy that model is saved for further use.

## Model Prediction
The following steps are performed here:
1. Loading the previously saved model(best model) from training phase.
2. Using webcam to generate test images and prediction is made.

Reload the page to play the below gif.

<img src="Demo.gif" title='face mask detection' width="750" align="center">
