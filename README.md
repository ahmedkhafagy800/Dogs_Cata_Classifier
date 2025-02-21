Overview
This project is a computer vision model that classifies images into two categories: cats and dogs. The model is built using TensorFlow and Keras, with MobileNetV2 as the base architecture. It is designed to predict whether an input image contains a cat or a dog.

Features
Image Preprocessing: Resizes and normalizes input images for compatibility with the model.

Deep Learning Model: Uses a pre-trained MobileNetV2 model fine-tuned for binary classification.

Prediction: Provides a probability score and a final classification (cat or dog) based on a user-defined threshold.

Visualization: Displays the input image using Matplotlib.

Model Architecture
The model is based on MobileNetV2, a lightweight and efficient convolutional neural network. The base model is pre-trained on ImageNet, and custom layers are added for binary classification.


Directory Structure:
cat-dog-classification/
├── data/
│   ├── train/
│   │   ├── cat/
│   │   └── dog/
│   └── test/
│       ├── cat/
│       └── dog/
├── models/
│   └── cat_dog_model.h5
├── predict_image.py
├── train.py
├── requirements.txt
├── README.md
└── LICENSE
