
# Electroencephalograms-during-Mental-Arithmetic-Task-Performance

## Overview

This task is centered around the analysis of EEG data to classify different cognitive states

using advanced deep learning techniques. The data is sourced from the Mental Arithmetic

Tasks Dataset available at PhysioNet (https://physionet.org/content/eegmat/1.0.0/). The

dataset is pre-cleaned and ready for use, allowing you to focus on model implementation

and evaluation. Please familiarize yourself with the dataset by reviewing the accompanying

research paper (https://www.mdpi.com/2306-5729/4/1/14).

  

## Data

The data files are provided in EDF (European Data Format) format. Each subject has two files:

  

- *_1: Recording of the background EEG (before the mental arithmetic task).

- *_2: Recording of the EEG during the mental arithmetic task.

The recording datetime information has been set to January 1 for all files.

  

## Subjects and Groups

The subjects are divided into two groups:

  

- Group "G": 24 subjects performing a good quality count (Mean number of operations per 4 minutes = 21, SD = 7.4).

- Group "B": 12 subjects performing a bad quality count (Mean number of operations per 4 minutes = 7, SD = 3.6).

The file subject-info.csv provides basic information about each subject (gender, age, job, date of recording) and indicates which subjects correspond to which group (0 - Group "B", 1 - Group "G").

  

## Getting Started

First, download the zip file, extract the dataset, and load the data using the MNE package in Python. This will allow us to visualize and perform operations on the EEG data.

  

## Objectives

Your goal is to implement and evaluate multiple deep learning models (at least two) using the Python library MNE. Your entire analysis should be documented in a Jupyter Notebook, which you’ll submit via a GitHub repository link.

  

## Steps to Achieve It

### 1. Load the EEG Data

Start by loading the EEG data into your environment using the MNE library.

  

### 2. Power Spectral Density (PSD) Analysis

a. Calculate the band-wise PSD for both states:

  

- Rest (recording EEG dataset before the mental arithmetic task)

- Task (recording of EEG dataset during the mental arithmetic task)

Focus on the following frequency bands:

  

- Delta (1-4 Hz)

- Theta (4-8 Hz)

- Alpha (8-12 Hz)

- Beta (12-30 Hz)

- Gamma (30-100 Hz)

b. Compare the PSDs of the two states and summarize your findings.

  

# 3. Deep Learning Classification

a. Extract relevant features from the cleaned data.

  

b. Implement binary classification using two different deep learning models. You can choose from:

  

 - EEGNet
   
  - TSCeption
   
  - ViT (Vision Transformer)
   
   - ATCNet
   
   - VAE (Variational Autoencoder)

c. Train and validate the models using the provided dataset.

  

d. Evaluate the models using appropriate metrics (accuracy, precision, recall, F1-score) and discuss the results.

## Submission Guidelines

● Ensure that your Jupyter Notebook is well-organized and thoroughly commented

● Share your completed notebook by submitting the GitHub repository link