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

Describe the architecture of your solution. This can include:

- **System Overview**: High-level description of the system's design and how the components interact.
- **Components**: Details about each major component and its role.
- **Data Flow**: Explanation of how data is processed, transformed, and utilized within the system.

Include diagrams if available:

![Architecture Diagram](images/architecture-diagram.png)
*Figure 1: System architecture diagram.*

## Tools/Models Used

List and describe the tools and models used in the project:

- **TensorFlow**: A powerful library for machine learning and deep learning tasks.
- **Apache Kafka**: A distributed event streaming platform used for real-time data processing.
- **Python**: The programming language used for implementing the project.

Provide links to documentation or resources for each tool/model if available.

## Installation

Follow these steps to set up the project on your local machine:

```bash
git clone https://github.com/username/repository.git
cd repository
pip install -r requirements.txt







