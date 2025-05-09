# Crop Disease Analysis Using Vegetation Indices and Attention-Based LSTM

## Overview

This project implements an end-to-end pipeline for analyzing crop health and disease patterns using multispectral vegetation index rasters. It covers:

- Loading and preprocessing raster files of vegetation indices (e.g., NDVI, EVI).
- Building a custom PyTorch **CNN + LSTM + Multi-Head Self-Attention** model to learn latent representations of vegetation patterns.
- Training and evaluating the model on labeled raster datasets.
- Extracting latent features and performing **K-Means clustering** to discover patterns in the data.
- Visualizing cluster assignments in 2D via **PCA**.

## Features

- **Custom Dataset** (`VegetationDataset`) to load multi-band raster files and optionally resize them.
- **Vegetation Indices Loader** using `rasterio`.
- **CNN + LSTM + Attention** architecture for spatio-temporal feature learning.
- **Clustering & Visualization** of learned latent representations.
- Modular code that can be adapted for other remote-sensing classification or clustering tasks.

## Requirements

- Python 3.7+
- [PyTorch](https://pytorch.org/)  
- torchvision  
- rasterio  
- numpy  
- scikit-learn  
- matplotlib  
- Pillow  
