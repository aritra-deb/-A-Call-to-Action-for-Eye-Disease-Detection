# -A-Call-to-Action-for-Eye-Disease-Detection

## Problem Statement

Imagine a world where the beauty of a sunset, the colors of a rainbow, or the joyful eyes of a loved one start to fade away, not due to the passage of time but because of a lurking ocular disease. The reality is that millions across the globe face this daunting experience daily, with conditions like CNV, DME, and Drusen leading the charge.

Harness the power of machine learning to train a model that accurately identifies and classifies these conditions.

## The Dataset – Arsenal for Change

Before you is a rich dataset, diligently segmented into four classes: CNV, DME, Normal, and Drusen. The training set boasts 5,000 images per class, allowing you to deep-dive into the intricacies of each condition. To refine and tune your models, a validation set of 1,000 images per class stands ready.

## What's Included

### Data Augmentations

These techniques defines a set of image transformations to augment the dataset. Data augmentation is a technique used to artificially increase the diversity of your training data, which can help improve model performance and reduce overfitting.
For the 'train' set (used during training), the following transformations are applied:
Resizing the images to 64x64 pixels.
Horizontal flipping of images with a 30% probability (50% chance of being flipped).
Random rotation of images up to 30 degrees.
Normalizing the pixel values with a mean of 0.5 and a standard deviation of 0.5.
Converting the images to PyTorch tensors.
For the 'val' (validation) and 'test' sets, similar transformations are applied, but without the horizontal flip.


## Training Results

| Model     | Epochs | Train Loss | Train Accuracy | Validation Loss | Validation Accuracy |
|-----------|--------|------------|----------------|-----------------|---------------------|
| ResNet-18 | 50     | 0.243785   | 0.911          | 0.362895        | 0.874               |
| ResNet-50 | 50     | 0.270888   | 0.899          | 0.415653        | 0.859               |
