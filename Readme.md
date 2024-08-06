# Planogram_Analysis

## Table of Contents

1. [Introduction](#introduction)
2. [Solution Architecture](#solution-architecture)
3. [Tools/Models Used](#toolsmodels-used)
4. [Installation](#installation)
5. [Results](#results)

## Introduction

The main objective of this usecase is to detect the SKU(store keeping units) and grouping similar SKU using the feature extraction algorithms and cosine similarity to create the clusters of same objects/products. For SKU detection, YOLOV5 model trained on SKU110 dataset has been used and in the next step the detected objects are passed to the feature extraction algorithms VGG16 and image hashing.In the end the clustering algoirthms are applied to cluster the extracted features using cosine similarity and hamming distance.

## Solution Architecture

The overview of the implementation is represented in the below diagram

- **SKU Detection**: In this application user needs to upload an Image that will detect SKU's using YOLOV5 Object detection model trained on SKU110 Dataset. Detected objects/products will be stored for next step(Feature Extraction) with their confidence level and co-ordinates in the image.
- **FeatureExtraction**: At this stage, Image Features Extraction is performed using multiple alogorithms(like VGG16, Image GPT and Image Hashing) on the original and enhanced detected objects.
- **Clustering**: Last step is to implement the clustering algorithms on the extracted features using cosine similarity and hamming distance.
Include diagrams if available:

![Architecture Diagram](images/architecture-diagram.png)
*Figure 1: System architecture diagram.*

## Models/Tools Used

The list of the models that are used for the implementation given below:

- **Model1**: YOLOV5 model to detect the store keeping unit(SKU).
- **Model2**: Feature extraction model to detect the products that are present in the SKU.


## Installation

Follow these steps to set up the project on your local machine:

```bash
cd repository
$ pip install -r requirements.txt

```
After installing all the required libraries, now let's run the file after opening terminal in src folder
```bash
$ streamlit run app.py


