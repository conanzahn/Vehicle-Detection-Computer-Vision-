# Vehicle Detection (Computer Vision - Individual Project)

## Preview

![VehicleDetect](https://user-images.githubusercontent.com/54277153/130087448-f9fcf60b-e445-4683-bfdd-b0120396c74e.jpg)

## Introduction
Vehicle detection and statistics are an important component
of computer vision. With the popular installation of traffic 
surveillance cameras, the use of computer vision for intelligent 
recognization and analysis of vehicles becomes very effective.
Vehicle detection takes images as input, analyzes through a 
series of algorithms, and outputs labelled images with bounding 
boxes around the recognized vehicles.

## [Dataset](https://github.com/TuSimple/tusimple-benchmark) (click here to access datasets)
The complexity of the dataset for this task is the video 
recorded on highways, vehicles with different relative distances, 
and variable traffic conditions. As for the size of datasets, the 
model training part using the training dataset which contains 
1074 clips of 2s videos in 20 frames per second and 3222 
annotated vehicles. Model evaluation part using the testing 
dataset which contains 269 clips of videos with the same format 
as training data.

## Challenge
The challenge of this technology is the complexity of the 
camera scene. When the vehicle appears in the photo at a far 
perspective, the target object occupies a small pixel, and the 
detection accuracy is low. When the vehicle appears in the close 
perspective in the photo, the target objects occupy large pixels; 
this causes a great change in the size of the target object.

## My Solution
I focus on the above issues to propose a viable 
solution, I apply the Histogram of Oriented Gradients to extract 
image features, select the support vector machine (SVM) as the 
classifier model to train the dataset.

## Method Structure
- Preprocessing of Dataset
    - Region of interest (ROI)
    - Resize dataset
- Feature Extraction
    - HOG feature extraction
- Classifier
    - support vector machine (SVM) 
- Object Detection
    - sliding window

## How to Use
1. Clone/Download the repo [https://github.com/conanzahn/Vehicle-Detection-Computer-Vision-.git]
2. Download Datasets to your local machine [https://github.com/TuSimple/tusimple-benchmark]
3. Run Jupyter notebook
