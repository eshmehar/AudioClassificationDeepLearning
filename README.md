# Audio Classification with CNN on UrbanSound8K Dataset

This project implements a deep learning model using a Convolutional Neural Network (CNN) for classifying urban sound events such as dog barks, gunshots, and street music. The model is trained on the [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html) dataset, leveraging audio features like Mel-Frequency Cepstral Coefficients (MFCCs) for sound classification.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Model Architecture](#model-architecture)
- [Results](#results)

## Project Overview
The goal of this project is to build a robust audio classification system using CNNs, which can classify various urban sound categories based on MFCC features extracted from audio samples. The system is designed to assist in tasks like urban sound monitoring, security, and surveillance.

## Dataset
The project uses the [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html) dataset, which contains 8,732 labeled sound excerpts of up to four seconds, categorized into 10 different urban sound classes:
- Air Conditioner
- Car Horn
- Children Playing
- Dog Bark
- Drilling
- Engine Idling
- Gunshot
- Jackhammer
- Siren
- Street Music

## Features
- **Audio Preprocessing**: Extracts MFCC features from raw audio files using the `librosa` library.
- **Deep Learning Model**: A Convolutional Neural Network (CNN) model is trained to classify sounds based on extracted MFCC features.
- **Visualization**: Plots showing accuracy and loss over epochs to track model performance.
- **Confusion Matrix**: Displays the classification results for each sound class.

## Model Architecture
The model is a Convolutional Neural Network designed for handling audio feature data:
- **Input Layer**: Takes MFCC features as input.
- **Convolutional Layers**: Extract spatial features from the MFCC input.
- **Dense Layers**: Final layers for sound category classification.
- **Output Layer**: Softmax activation for multi-class classification.

## Results
- **Test Accuracy**: 90.10%
- **Training vs Test Accuracy**: Consistent improvement with a small gap indicating good generalization.
- **Confusion Matrix**: Shows high accuracy in several classes but also highlights areas for improvement, particularly in distinguishing between similar sound categories.
