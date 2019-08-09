# Sentiment Analysis

## Overview
This project is a basic form of NLP which classifies movie reviews from the IMDb dataset as either positive or negative. 

Some of the challenging aspects of this project are:
1. Reviews such as **"This is not a good movie"** has a negative meaning but depending on the parameters learned in the network, the word "good" might be used to distinguish the sentiment or in other words the network has to learn to extract meaning from the order of multiple words such as "not good" and not treat each word independently.
2. Neural networks can't work directly on text data, so it needs to be converted to a compatible format.
3. The sequences or the reviews can be of arbitrary length

This project can also be converted to a star rating system i.e excellent being 5 star, good being 4 star, neutral being 3 star and so on by having an appropriate dataset and using a softmax function instead of sigmoid as the activation for the output layer. 

## Flowchart
![flowchart](https://user-images.githubusercontent.com/45155542/62746504-f3e1f300-ba1d-11e9-88d9-68dac4e987db.PNG)

**Credit: Hvass-Labs**

## Architecture
I've used a 3 layered RNN (Recurrent Neural Network) with GRUs (Gated Recurrent Unit) as the recurrent unit.

The architechture is as shown below:
![architechture](https://user-images.githubusercontent.com/45155542/62746482-da40ab80-ba1d-11e9-8644-5843f2f1b3cb.PNG)

**Credit: Hvass-Labs**

## Accuracy
I was able to achieve around 90% accuracy on the test/dev set. It can be further improved by:
1. Using a deeper network
2. Increasing the dimensions of the embedding vectors
3. Training for higher number of epochs
4. Getting more data

## System requirements
1. Jupyter notebook
2. Keras
3. Tensorflow
4. numpy

## How to run
The source file (One .ipynb file) and dataset files (Two .py files) should be downloaded into the same folder. Run all the cells in the source file.

