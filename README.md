# MoA_competition
The solution of the mechanism of action prediction competition on kaggle in collaboration with [@Nicohrubec](https://github.com/nicohrubec). **The models in this repository work perfectly with tabular data with multi-label targets**

### BLOG POST: https://medium.com/@aminey/drug-discovery-with-neural-networks-a6a68c76bb53

A summary of the Mechanisms of action (MoA) prediction competition on kaggle where we used deep learning algorithms to predict the MoA of new drugs. This repository includes the models, training pipeline, weights and inference pipeline.

## 1- Models:
> ### 1- Multi layer perceptron:
A simple feed forward neural network, the simplest neural networks architecture with 4 dense layers (first 2 layers with 2048 neurons and the last two with 1048 neurons)
![alt text](https://raw.githubusercontent.com/Amiiney/MoA_competition/main/moa_mlp-8.png)
Parameters: Adam optimizer, Reduce on plateau scheduler and a binary cross-entropy BCE With Logits Loss function that includes a sigmoid activation.

> ### 2- TabNet:
TabNet is a deep learning model for tabular data. TabNet combines the properties of neural networks and tree-based algorithms.


> ### 3- DeepInsight image transformation + EfficientNet B4
Tabular data is transformed to t-SNE image data and fed to an efficientNet B4 model.

# 2- Training models:
In order to train the models (MLP, TabNet, DeepInsight B4) you need to attach the corresponding datasets to your jupyter notebook. Links to the datasets are available in the first markdown of each notebook.
