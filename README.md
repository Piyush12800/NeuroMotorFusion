# NeuromotorFusion

NeuromotorFusion is a project that implements two deep learning classification models, EEGNet and ShallowFBCNet, for analyzing the BCI Competition IV 2a dataset. The goal is to classify motor imagery tasks based on EEG data. The project uses the PhysioNet dataset for the EEGNet model and Braindecode's MOABBDataset for the ShallowFBCNet model.

## Table of Contents
- [Introduction](#introduction)
- [Datasets](#datasets)
- [Models](#models)
- [Installation](#installation)

## Introduction
NeuromotorFusion is designed to classify EEG signals from the BCI Competition IV 2a dataset, a popular dataset for motor imagery classification. Two architectures are explored:
1. **EEGNet**: A compact CNN model for EEG-based BCI, using PhysioNet data.
2. **ShallowFBCNet**: A shallow convolutional network from Braindecode, using Braindecode's MOABBDataset.

## Datasets
### BCI Competition IV 2a Dataset
The dataset includes EEG recordings from 9 subjects performing four different motor imagery tasks: left hand, right hand, feet, and tongue. For the models:
- **EEGNet**: Data is sourced from [PhysioNet](https://physionet.org/).
- **ShallowFBCNet**: Data is sourced using [Braindecode's MOABBDataset](https://braindecode.org/).

## Models
### EEGNet
EEGNet is a lightweight neural network architecture that performs well on BCI tasks. It uses depthwise and separable convolutions to learn spatial and temporal features from EEG data.

### ShallowFBCNet
ShallowFBCNet is a simpler, single-layer convolutional neural network designed to perform robustly on EEG data with minimal preprocessing. It uses band-pass filtering and exponential moving standardization to enhance features.

## Installation
To install the required dependencies, clone the repository and run:

```bash
git clone https://github.com/Piyush12800/NeuroMotorFusion.git
cd NeuromotorFusion
pip install -r requirements.txt
