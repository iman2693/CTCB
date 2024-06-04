# CTCB (Classification of Toxigenic CyanoBacterial genera)
Automated identification of toxigenic cyanobacterial genera for quality control purposes =>  [Paper Link](https://www.sciencedirect.com/science/article/pii/S030147972401260X?dgcid=author)
## Introduction :
This repository is for introducing and sharing the TCB dataset and codes were used in the [paper](https://github.com/iman2693/CTCB). 

## Compatibility
The code is tested using Tensorflow 2.8, Cudnn 8.1.0.77, Cuda 11.2, and Python 3.8 .

## Requirements:
* keras
* tensorflow
* numpy
* matplotlib
* pandas
* plotly
* scikit-learn

## Dataset:
The TCB dataset is available from the corresponding authors for follow up studies. The TCB-DS dataset is a specialized collection of microscopic images focusing on the automatic recognition of cyanobacteria genera. This dataset was meticulously compiled to address the challenges associated with the varying image qualities due to differences in contrast, resolution, size, lighting, and the presence of noise in the original images. It includes 2,591 images with varying dimensions, ranging from a minimum of 11 × 41 pixels to a maximum of 5184 × 3456 pixels, with a mode size of 150 × 150 pixels. The images were sourced from multiple reputable databases and were manually cropped to remove unsuitable samples, ensuring that the dataset contains only relevant and high-quality images. The TCB-DS dataset was then divided into training and test sets with an 80:20 split. More details about the dataset and how it was collected are mentioned in the paper.
#### Training Set:
Training Set of TCB dataset includes 2,073 images.
#### Test Set:
Training Set of TCB dataset includes 518 images.

## Fine-tuned models
| Model name      | Weighted f1-score | Macro f1-score | Architecture |
|-----------------|--------------|------------------|-------------|
| [Model 1](https://github.com/iman2693/CTCB/tree/main/weights/Model1%20-%20MobileNet) | 0.9491        | 0.8353    | Model 1 (MobileNet) |
| [Model 2](https://github.com/iman2693/CTCB/tree/main/weights/Model2%20-%20MobileNetV2) | 0.9293        | 0.8764      | Model 2 (MobileNetV2)|


