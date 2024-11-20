# aiIsMyth_ML_Project

Problem Statement

The project is somewhat inspired by the this problem statement [here](https://www.sciencedirect.com/science/article/pii/S2772375523000515). 

## Overview

This repository contains the project for the course CS550: Machine Learning, which is a part of the curriculum for the semester 2024-25M at IIT Bhilai. The objective of this project is to build a machine learning model for classification using ResNet50, efficientNet and VGG19 pretrained models via transfer learning. The goal is to leverage these resources to build an ensemble model for improved performance

## Data Collection

The dataset is sourced from two different sources, [source1](https://zenodo.org/records/5801834) and [source2](https://zenodo.org/records/4628934).
Each source provides labeled images corresponding to different diseases, with various file formats and resolutions. The dataset has been pre-processed to make it compatible with the models used in this project.


## ROI extraction

In this project, Region of Interest (ROI) extraction plays a crucial role in improving the model's performance by focusing on the most relevant parts of the images. We have used YOLOv5 (You Only Look Once version 5), a state-of-the-art object detection model, for efficient and accurate extraction of the regions of interest from the dataset.

## Transfer Learning

In this project, we utilized ResNet50, efficienNet and VGG19, all of which are popular and powerful convolutional neural networks (CNNs) pre-trained on the ImageNet dataset. These models have shown excellent performance on various image classification tasks and were fine-tuned on our custom dataset to classify images based on specific disease categories.

## Ensemble Model with majority voting

To further improve the model’s performance, we created an ensemble model that combined the predictions from all models. By using the predictions from three models, the ensemble model leverages the strengths of each individual model, often leading to a better overall classification performance. The ensemble strategy typically involves averaging the output probabilities of each model, or voting based on the predicted class labels.
