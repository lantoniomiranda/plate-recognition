# License Plate Recognition Project

## Overview

This project focuses on recognizing license plates using deep learning models. The notebook includes steps to train and deploy a YOLO (You Only Look Once) model for license plate detection.

## Dataset

The dataset used for this project can be found at the following link:
[License Plate Detection Dataset](https://universe.roboflow.com/haeun-kim-ri91b/license-plate-detection-wienp/dataset/2)

## Requirements

- Install the necessary libraries: `torch`, `opencv-python`, and `ultralytics`.
- Configure the device to use GPU if available.
- Train the YOLO model using the provided dataset.
- Save the trained model for future use.
- Implement prediction and detection of license plates in images or videos.

## Run

### Input

I used a general video for input, found on internet.
Tried with other videos and also worked.

### Model Training

Once you hit run, the dependencies will be installed, and the model will be trained. With this configuration, it took around 2 hours to train the model, running with Colab Pro on an NVIDIA L4. Expect longer times with less powerful machines.

### Output

The project will generate 3 output videos:
1. The first video with 10% confidence on the detection.
2. The second video with 50% confidence on the detection.
3. The last run will use EasyOCR to read the text on the plates and also detect the color of the vehicle (note: color detection is not fully accurate yet).

