# Deforestation Detection Using Multi-Temporal NDVI and Attention U-Net

## Abstract

This project presents an automated deep learning framework for detecting deforestation using multi-temporal satellite imagery. The system computes NDVI (Normalized Difference Vegetation Index) from Sentinel-2 satellite data to analyze vegetation changes over time. An Attention U-Net model is used for pixel-wise segmentation of deforested regions. Monte Carlo Dropout is applied during inference to estimate uncertainty, and a risk scoring mechanism is used to classify regions into low, medium, and high-risk zones.

---

# System Architecture

Satellite Data
↓
Preprocessing
↓
NDVI Computation
↓
Patch Extraction
↓
Dataset Preparation
↓
Attention U-Net Model
↓
Prediction
↓
Uncertainty Estimation
↓
Post-processing
↓
Risk Mapping
↓
Visualization

---

# Technologies Used

* Python
* Jupyter Notebook
* PyTorch
* NumPy
* Pandas
* Matplotlib
* Rasterio
* OpenCV
* SciPy
* Git & GitHub

---

# Dataset Preparation

* Satellite image size: 10980 × 10980
* NDVI generated using Red and NIR bands
* Multi-temporal NDVI stack with 5 time steps
* Patch size: 256 × 256
* Total extracted patches: 1764
* Filtered patches: 162

---

# Algorithms & Techniques Used

* NDVI Computation
* Attention U-Net
* Binary Cross Entropy Loss
* Dice Loss
* Monte Carlo Dropout
* Threshold-based Segmentation
* Morphological Smoothing
* Risk Score Classification

---

# Results

* Epochs: 30
* IoU Score: 0.0016
* Dice Score: 0.0032
* Risk Score Range: 0.0027 – 0.80

---

# Future Improvements

* Increase dataset size
* Improve segmentation accuracy
* Deploy as a web application
* Add real-time monitoring
* Use transformer-based models

---

# GitHub Repository

This repository contains:

* Source code
* Jupyter notebooks
* Output visualizations
* Risk maps
* Final results
* Project documentation
