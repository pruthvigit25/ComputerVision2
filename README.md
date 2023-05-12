# Strawberry Ripeness Detection and Classification using YOLOv5

This repository contains the code and resources for a study on accurate detection and classification of strawberry ripeness using the YOLOv5 object detection model.

## Background

The study builds upon previous approaches to object detection, including traditional methods such as SIFT and SURF, as well as more recent methods such as faster R-CNN and YOLOv3. YOLOv5 is a state-of-the-art object detection model that has demonstrated high accuracy and fast processing speeds on various tasks. Previous studies have shown the success of YOLOv5 in object detection for autonomous vehicles, security systems, and satellite imagery.

## Implementation

The model was implemented using a dataset of images containing strawberries in different stages of ripeness. Each image was labeled with bounding boxes and a ripeness class ID (0 = unripe, 1 = partially ripe, 2 = fully ripe). The YOLOv5 model was trained using supervised learning, with image size set to 416x416 pixels, batch size of 16, and 100 epochs.

## Results

The performance of the model was evaluated on a separate dataset, and the accuracy and speed were measured. The model achieved an overall accuracy of 95.80% in classifying strawberry ripeness and counting the number of strawberries in each image. The results were visualized using Tensor Board and Python's OpenCV library.


## Repository Structure

- `data/`: Contains the dataset of strawberry images and annotations.
- `models/`: Includes the pre-trained YOLOv5 model and the custom configuration file.
- `train.py`: Code for training the YOLOv5 model.
- `test.py`: Code for evaluating the model's performance on the test dataset.
- `utils/`: Utility functions for data processing and evaluation.

## Requirements

- Python 3.x
- PyTorch
- OpenCV
- NumPy

## Usage

1. Clone the repository:

```shell
git clone https://github.com/your-username/strawberry-ripeness-detection.git

2.Install the required dependencies:
pip install -r requirements.txt

3.Prepare the dataset and annotations in the data/ directory.
4.Train the model:
python train.py

5.Test the model:
python test.py
