# Age and Gender Prediction Using ResNet50

## Overview
This project utilizes the ResNet50 architecture to build a multi-output model for predicting:
- **Age** (as a regression task)
- **Gender** (as a binary classification task)

The model is trained on the [UTKFace Dataset](https://www.kaggle.com/datasets/jangedoo/utkface-new), a large dataset of aligned and cropped facial images with age and gender labels.

## Features
- Multi-output neural network leveraging transfer learning with ResNet50.
- Custom data generators for efficient batch processing.
- Loss functions tailored for age regression and gender classification.
- Customizable architecture for further improvements.

## Dataset
The [UTKFace Dataset](https://www.kaggle.com/datasets/jangedoo/utkface-new) contains:
- Aligned and cropped images of human faces.
- Labels for age and gender.

### Download Dataset
1. Place the `kaggle.json` file in your working directory.
2. Run the following commands in your notebook or environment:
   ```bash
   !mkdir -p ~/.kaggle
   !cp kaggle.json ~/.kaggle/
   !kaggle datasets download -d jangedoo/utkface-new
