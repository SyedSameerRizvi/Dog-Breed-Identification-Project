# 🐶 Multi Class Dog Breed Classification Project
This project demonstrates building an end-to-end multi-class image classifier using TensorFlow 2.0 and TensorFlow Hub. The task is to identify the breed of a dog given an image, which involves deep learning techniques and transfer learning.

## 1. Problem
The objective of this project is to classify the breed of a dog from a given image. The challenge is part of the Kaggle competition Dog Breed Identification.

Kaggle Competition: [Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification/overview)

**NOTE: Use Google Colab's GPU for faster runtime.**

## 2. Dataset
The dataset used is from the Kaggle competition mentioned above. It consists of thousands of images, with each image corresponding to one of 120 different dog breeds.

* Training Set: Contains images labeled with their corresponding breed.
* Test Set: Contains images for which breed labels are to be predicted.
* The dataset has a total of 120 breeds and around 10,000 images in the test set.
The data was uploaded and unzipped in the notebook from Kaggle.

**NOTE: I had a problem while unzipping the data into my google colab and google drive, There were some missing files in my train folder, so I lowered it down to 7890..**

## 3. Evaluation
The evaluation for this task is based on a multi-class classification metric, where the output is a file containing the prediction probabilities for each dog breed for every test image. You can refer to the[ evaluation criteria](https://www.kaggle.com/c/dog-breed-identification/overview/evaluation) on Kaggle.

## 4. Features and Approach
### Data Prepocessing
* The images were transformed into numerical tensors suitable for deep learning models.
* The project made use of Transfer Learning to leverage pre-trained models from TensorFlow Hub to improve accuracy and reduce training time

### Model Architecture
The notebook utilizes a pre-trained convolutional neural network (CNN) from TensorFlow Hub to extract features from the images and then applies fully connected layers to classify the breeds.

### Training
* The data was split into training and validation sets.
* The model was trained on labeled images, and its performance was evaluated based on accuracy and loss metrics.

## 5. Installation and Setup
### Requirements:
* Python 3.x
* TensorFlow 2.x
* TensorFlow Hub
* Pandas
* Matplotlib

## 6. Results
The notebook produces a model capable of classifying dog breeds with high accuracy. You can view the training process, including visualizations of loss and accuracy, in the notebook.
