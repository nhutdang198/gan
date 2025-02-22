# Deep Convolutional GAN (DCGAN) Project

This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) for image generation. The main goal of the project is to train a GAN to generate realistic images from random noise.

## Table of Contents

- [Deep Convolutional GAN (DCGAN) Project](#deep-convolutional-gan-dcgan-project)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Project Structure](#project-structure)
  - [Requirements](#requirements)
  - [Usage](#usage)
  - [Training](#training)
        - [Data Preparation:](#data-preparation)
        - [Model Architecture:](#model-architecture)
        - [Training:](#training-1)
        - [Progress Monitoring:](#progress-monitoring)
  - [Results](#results)

## Introduction

Generative Adversarial Networks (GANs) are a class of machine learning frameworks designed by Ian Goodfellow and his colleagues in 2014. GANs consist of two neural networks, a generator and a discriminator, which compete against each other in a zero-sum game. The generator creates fake data, while the discriminator tries to distinguish between real and fake data. Over time, the generator improves its ability to create realistic data, and the discriminator improves its ability to detect fake data.

This project focuses on implementing a DCGAN, a type of GAN that uses convolutional layers in both the generator and discriminator to capture spatial hierarchies in the data, making it particularly effective for image generation tasks.

## Project Structure
deep-convolutional-gan/ 
│ 
├── dataset/ # Directory containing the training dataset 
├── models/ # Directory to save trained models 
├── progress/ # Directory to save progress images during training 
├── deep-convolutional-gan.ipynb # Jupyter Notebook with the implementation 
├── README.md # Project README file 
└── requirements.txt # List of dependencies


## Requirements

To install the required dependencies, run:

```sh
pip install -r requirements.txt

```

## Usage

Clone the repository
``` sh

git clone https://github.com/nhutdang198/deep-convolutional-gan.git
cd deep-convolutional-gan

```

Prepare the dataset:

- Login to kaggle account
- Run kaggle command to download dataset
- Run extract.ipynb to extract dataset

Run the Jupyter Notebook:

Open deep-convolutional-gan.ipynb in Jupyter Notebook or Jupyter Lab and follow the instructions to train the DCGAN.

## Training
The training process involves the following steps:

##### Data Preparation:
Load and preprocess the dataset of images from the specified dataset_path.

##### Model Architecture:
Define the generator and discriminator models using convolutional layers.

##### Training:
Train the GAN using the specified hyperparameters. The training process involves alternating between training the discriminator and the generator.

##### Progress Monitoring:
Save generated images at regular intervals to the progress/ directory to monitor the training progress.

Save the trained models to the models/ directory for future use.

## Results

During training, generated images will be saved in the progress/ directory. You can visualize the progress of the generator in creating realistic images over time.

