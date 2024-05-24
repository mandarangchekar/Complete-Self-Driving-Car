# Complete Self-Driving Car

This project simulates a fully functional self-driving car model using Convolutional Neural Networks (CNN) and Computer Vision. The model can correctly predict turns and stops, identify traffic signs, and drive without unwanted stops and crashes.

[Link to simulator video](https://www.linkedin.com/posts/mandar-angchekar_datadriven-deeplearning-ml-activity-6673940751577157632-1PKL?utm_source=share&utm_medium=member_desktop)

## Project Overview

- **Model**: Convolutional Neural Network (CNN)
- **Techniques**: Dimensionality reduction (correlation matrix, PCA, SVD)
- **Dataset**: [Track Dataset](https://github.com/mandarangchekar/Track)
- **Framework**: Keras

## Files in the Repository

- `Behavioural_Cloning.ipynb`: Jupyter Notebook containing code and explanations for training the self-driving car model using behavioral cloning.
- `README.md`: This file, providing an overview and instructions for the project.
- `drive.py`: Python script for running the trained model to control the car in a simulated environment.
- `model.h5`: Saved Keras model in HDF5 format, containing the trained neural network.

## Getting Started

### Prerequisites

Ensure you have the following libraries installed:
- Python
- Keras
- TensorFlow
- NumPy
- OpenCV
- Flask
- SocketIO
- Eventlet
- PIL

### Installing

Clone the repository and navigate to the project directory:
```sh
git clone https://github.com/mandarangchekar/Complete-Self-Driving-Car.git
cd Complete-Self-Driving-Car
```

Running the Model
Train the Model:
Open Behavioural_Cloning.ipynb and run all the cells to train the model. The trained model will be saved as model.h5.

Run the Simulation:
Use the drive.py script to run the trained model in a simulated environment.

```sh
python drive.py
```

# Code Details

## Behavioural_Cloning.ipynb

This notebook includes the following steps:

### Data Loading and Preprocessing:
- Loading images and steering angles from the dataset.
- Preprocessing images (cropping, resizing, normalizing).

### Data Augmentation:
- Augmenting data to create a more robust model.

### Model Definition:
- Defining the CNN architecture based on the NVIDIA model.

### Training:
- Training the model using the preprocessed and augmented data.

### Evaluation:
- Evaluating the model's performance and saving the trained model.

## drive.py

This script sets up a server to communicate with the simulator and control the car using the trained model:

### Image Preprocessing:
- Cropping, resizing, and normalizing incoming images from the simulator.

### Model Prediction:
- Using the trained model to predict steering angles.

### Sending Control Commands:
- Sending steering and throttle commands to the simulator.

## Results

The trained model can successfully identify between 43 different traffic signs and drive without unwanted stops and crashes, demonstrating its effectiveness in a simulated environment.
