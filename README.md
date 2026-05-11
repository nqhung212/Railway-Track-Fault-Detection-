# Railway Track Damage Detection using Deep Learning

## Overview

This repository implements an automated railway track defect detection system using image classification. Two approaches are included: a fine-tuned ResNet50 model and a hybrid pipeline that uses ResNet50 as a feature extractor with a Kernel SVM classifier.

## Dataset

Images are labeled into two classes: Defective and Non-Defective. The report references the Railway Track Fault Detection dataset from Kaggle. Place the dataset into the expected train/validation/test folders before running the notebooks.

## Methods

- resnet50_new.ipynb: fine-tunes a pre-trained ResNet50 in four phases to improve generalization.
- svm_newest.ipynb: extracts 2048-dim features from ResNet50 and classifies them using an SVM optimized with GridSearchCV.

## Results

- ResNet50 fine-tuning: ~95.5% test accuracy.
- ResNet50 features + Kernel SVM: ~90.9% test accuracy.

## Setup and Run

1. Create a Python environment and install dependencies:
   ```bash
   pip install tensorflow scikit-learn opencv-python matplotlib seaborn jupyter
   ```
2. Launch Jupyter and open the notebooks:
   ```bash
   jupyter notebook
   ```