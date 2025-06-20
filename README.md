﻿# SmallWT_Fb
## Data Collection

- Capture images or video frames of the wind tunnel experiments.
- Ensure consistent lighting and camera positioning for easier processing.

## Data Labeling

- Manually create pixel-wise segmentation masks for the images, labeling firebrands, flames, and background.
- Tools such as CVAT or Labelbox can help with annotation.

## Preprocessing

- Normalize image sizes, apply color corrections, or crop regions of interest.
- Augment the data (flips, rotations, brightness changes) to increase variation.

## Model Training

- Implement or adapt a UNet architecture using a framework like PyTorch or TensorFlow.
- Split the data into training, validation, and test sets.
- Optimize the model with a suitable loss function (e.g., cross-entropy with dice loss).

## Evaluation

- Assess accuracy using metrics such as Intersection over Union (IoU) or F1 score for each class (firebrand, flame, background).
- Visualize predictions compared to ground truth to identify failure cases.
