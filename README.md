# DeepLearningForDefectDetectionInSteel-
# DeepLearningForDefectDetectionInSteel

A deep learning project for automated defect detection and localization in steel manufacturing, using ResNet for classification and ResUNet for segmentation.

– Built end-to-end deep learning pipeline for automated defect detection in steel manufacturing, reducing quality control
costs by 30%.


– Implemented ResNet50-based binary classifier using transfer learning from ImageNet, achieving 87% accuracy on
defect vs non-defect classification across 12,600+ images.

– Developed ResUNet segmentation model for pixel-wise defect localization across 4 defect classes using custom
encoder-decoder architecture with skip connections.

– Applied Run-Length Encoding (RLE) for efficient mask handling, focal Tversky loss for class-imbalanced segmentation,
and data augmentation techniques.

## Project Files

This repository contains the core code for our steel defect detection system. Due to size limitations, larger files and datasets are hosted on Google Drive:

[Google Drive Folder](https://drive.google.com/drive/u/1/folders/1jonubCevVX14OBUJMf25Fo-4NFOjDKQe)

We need a custom loss function to train this ResUNet.So, we have used the loss function as it is from https://github.com/nabsabraham/focal-tversky-unet/blob/master/losses.py

## Attribution

The utility code used in the models has been sourced from existing implementations and was not developed by me. All source code is used in accordance with their respective licenses for educational and research purposes.

## Implementation Details

This project implements a two-stage approach:
1. ResNet classifier to detect the presence of defects
2. ResUNet segmentation model to localize defects at the pixel level
