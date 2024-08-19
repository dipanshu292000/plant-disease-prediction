Plant Disease Prediction Using CNN

This project implements a Convolutional Neural Network (CNN) to classify and predict plant diseases based on images. 
The model is trained on the PlantVillage dataset, which contains labeled images of healthy and diseased plant leaves.
The goal is to develop a robust image classifier that can identify the type of disease affecting a plant from an image of its leaf.

Dataset

Dataset Source:
The dataset used in this project is the PlantVillage dataset, which is downloaded from Kaggle.

Dataset Structure:
The dataset is organized into three folders—segmented, color, and grayscale—each containing images of plant leaves. 
The color folder, which contains color images, is used for training and validation in this project.

Number of Classes:
The dataset includes 38 different classes, each representing a specific plant disease or a healthy plant condition.

Project Workflow

Environment Setup:
The Kaggle API key is set up to download the dataset.
The dataset is extracted from a zip file and organized into appropriate directories.


Data Preprocessing:
Images are preprocessed using the ImageDataGenerator class from TensorFlow's Keras API.
Images are rescaled, and the dataset is split into training and validation sets, with 20% of the data reserved for validation.


Model Architecture:
A Convolutional Neural Network (CNN) is built using TensorFlow's Keras library.
The model consists of several convolutional layers followed by max-pooling layers and fully connected dense layers.


Training:
The model is trained on the preprocessed images with the Adam optimizer and categorical cross-entropy loss function.
The model's performance is monitored using validation data, and accuracy metrics are calculated.


Evaluation:
The trained model is evaluated on the validation set to determine its accuracy in classifying plant diseases.
The model's performance is visualized using loss and accuracy plots.


Prediction:
The trained model can be used to predict the disease class of new plant leaf images by feeding them through the model.
