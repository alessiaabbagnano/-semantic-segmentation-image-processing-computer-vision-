# Semantic Segmentation for Image Processing and Computer Vision

## Project Overview
This project addresses the problem of **semantic segmentation**, i.e., the assignment of a semantic class to each pixel of an image. The goal is to analyze and compare different deep learning approaches in terms of performance, generalization, and interpretability.

## Methods
The following approaches have been implemented and evaluated:

- **U-Net (from scratch)** trained on the Cityscapes dataset
- **DeepLabV3 with ResNet-50 backbone**, fine-tuned on Cityscapes
- **Transfer Learning approach**, where a U-Net pre-trained on Cityscapes is adapted to COCO-Stuff 2017
- **Zero-shot evaluation** using the foundation model Meta Segment Anything 2 (SAM 2)

## Evaluation
The models were evaluated using both quantitative and qualitative metrics:

- Mean Intersection over Union (mIoU)
- Training and validation loss
- Qualitative analysis of predicted segmentation masks
- Confusion matrices

## Interpretability
An **Activation Maximization** technique was implemented to analyze and interpret the learned features of the U-Net model. This allowed an investigation of how internal representations evolve across the encoder, bottleneck, and decoder stages.

## Datasets
- Cityscapes
- COCO-Stuff 2017

## Notes
This repository is intended for research and educational purposes.
