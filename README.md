# Cat and Dog Image Classification

## Overview
This project is a computer vision model that classifies images into two categories: **cats** and **dogs**. The model is built using TensorFlow and Keras, with MobileNetV2 as the base architecture. It is designed to predict whether an input image contains a cat or a dog.

## Features
- **Image Preprocessing**: Resizes and normalizes input images for compatibility with the model.
- **Deep Learning Model**: Uses a pre-trained MobileNetV2 model fine-tuned for binary classification.
- **Prediction**: Provides a probability score and a final classification (cat or dog) based on a user-defined threshold.
- **Visualization**: Displays the input image using Matplotlib.

## Model Architecture
The model is based on **MobileNetV2**, a lightweight and efficient convolutional neural network. The base model is pre-trained on ImageNet, and custom layers are added for binary classification.

### Model Summary
```plaintext
Model: "model"
_________________________________________________________________
Layer (type)                 Output Shape              Param #
=================================================================
input_1 (InputLayer)         [(None, 120, 120, 3)]     0
mobilenetv2_1.00_224 (Functi (None, 4, 4, 1280)        2257984
global_average_pooling2d (Gl (None, 1280)              0
dense (Dense)                (None, 128)               163968
dropout (Dropout)            (None, 128)               0
dense_1 (Dense)              (None, 1)                 129
=================================================================
Total params: 2,421,081
Trainable params: 164,097
Non-trainable params: 2,256,984

datasets/
├── json-file14/
│   ├── kaggle.json
├── user-data/
│   ├── cat.jpg
│   ├── dog.jpg
│   ├── dog2.jpg
│   ├── luca1.jpg
│   ├── luca2.jpg
│   ├── luca3.jpg
│   ├── peter-cat.jpg
└── output (2.5GiB / 19.5GiB)/
    ├── kaggle/working/
    │   ├── dogs-vs-cats.zip
    │   ├── sampleSubmission.csv
        ├── test1/
    │   ├── test1.zip
    │   ├── train/
    │   ├── train.zip



Dataset
The model is trained on a dataset of cat and dog images. You can use your own dataset or download one from Kaggle.

Training Data: /kaggle/working/train -> which model train on it 

Testing Data: /kaggle/working/test1 -> which model tested by it

Online-img: /kaggle/input/user-data -> user can pass its pass at the last cell to test the model


