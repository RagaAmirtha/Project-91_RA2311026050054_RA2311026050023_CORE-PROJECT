# Deforestation Detection Using Multi-Temporal NDVI and Attention U-Net

# Abstract

Deforestation is a major environmental issue affecting biodiversity, climate stability, and ecosystem balance. This project presents an automated deep learning-based framework for detecting deforestation using multi-temporal satellite imagery. The system computes the Normalized Difference Vegetation Index (NDVI) from Sentinel-2 satellite data to analyze vegetation changes over time. An Attention U-Net segmentation model is used to identify deforested regions at the pixel level. Monte Carlo Dropout is applied during inference to estimate prediction uncertainty, improving model reliability. A risk scoring mechanism is also implemented to classify regions into low, medium, and high-risk zones. The proposed system generates segmentation outputs, uncertainty maps, and risk classification maps for environmental monitoring and decision-making.

# Modules
Input Satellite Imagery (Sentinel-2)
NDVI Computation
Multi-temporal Feature Extraction
Patch Extraction (256×256)
Attention U-Net Segmentation
Monte Carlo Dropout
Risk Classification
Visualization and Output Generation

# Technologies Used
Technology	Purpose
Python	Core project implementation
Jupyter Notebook	Development environment
PyTorch	Deep learning model
NumPy	Numerical operations
Pandas	Data processing
Matplotlib	Visualization
Rasterio	Satellite image processing
OpenCV / SciPy	Post-processing
Git & GitHub	Version control
Dataset Preparation
Satellite image size: 10980 × 10980
NDVI generated from Red and NIR bands
Multi-temporal NDVI stack with 5 time steps
Patch size: 256 × 256
Total patches extracted: 1764
Filtered patches with deforestation pixels: 162

# Algorithms & Techniques Used
NDVI Computation
Attention U-Net
Binary Cross Entropy + Dice Loss
Monte Carlo Dropout
Threshold-based Segmentation
Morphological Smoothing
Risk Score Classification

# Results
Metric	Value
Epochs	30
IoU Score	0.0016
Dice Score	0.0032
Risk Score Range	0.0027 – 0.80
Output Generated
NDVI Visualization
Patch Extraction Visualization
Ground Truth vs Prediction
Uncertainty Map
Risk Classification Map


# Future Improvements
Increase dataset size for better learning
Improve segmentation accuracy
Integrate cloud deployment
Use advanced transformer-based architectures
Develop real-time monitoring system
GitHub Repository
