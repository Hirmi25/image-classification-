<h1>🚀 Image Classification using Deep Learning (CIFAR-10)</h1>

<h3>📌 Overview</h3>
This project implements an image classification model using deep learning and Convolutional Neural Networks (CNNs). The model is trained on the CIFAR-10 dataset, which consists of 60,000 color images categorized into 10 classes.

The model is built using TensorFlow/Keras, with backpropagation for weight optimization, the Adam optimizer for adaptive learning, and Sparse Categorical Crossentropy as the loss function. The goal is to develop an efficient image classifier with high accuracy.

<h3>✨ Features
🖼 Dataset: CIFAR-10</h3>
-Contains 60,000 images of 10 object classes:
🚀 airplane | 🚗 automobile | 🐦 bird | 🐱 cat | 🦌 deer | 🐶 dog | 🐸 frog | 🐎 horse | 🚢 ship | 🚚 truck

-Each image is 32x32 pixels, with 3 color channels (RGB).

-Data is preprocessed by normalizing pixel values to the range [0,1] for better model performance.

<h3>🏗 Model Architecture</h3>

The CNN model follows a deep learning-based feature extraction approach:

-Input Layer: 32x32 RGB images
-Convolutional Layers:
Conv2D layers with 32, 64, and 128 filters (3×3 kernels)
Batch Normalization for stable training
ReLU Activation for non-linearity

MaxPooling (2×2) to reduce spatial dimensions

-Fully Connected Layers:
Flattening layer
1024-neuron dense layer (ReLU)
Dropout (0.2) to prevent overfitting
Softmax output layer (10 categories)


<h3>🎯 Training Details</h3>
Loss Function: Sparse Categorical Crossentropy (for integer-labeled multi-class classification)

Optimizer: Adam (Adaptive Learning Rate)

Epochs: 50
Batch Size: 32

Data Augmentation:
Random horizontal flips
Random width and height shifts

<h3>📊 Evaluation Metrics</h3>

Training & validation accuracy are plotted over epochs.

Loss curves help in analyzing model performance.

Predictions are compared with ground truth labels.
