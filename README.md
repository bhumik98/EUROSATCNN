# Using CNN algoritm to classify Europe satellite images 
Image Dataset : https://www.kaggle.com/datasets/apollo2506/eurosat-dataset

This repository contains code for training a convolutional neural network (CNN) to classify satellite images from the EuroSAT dataset.

EuroSAT dataset

The EuroSAT dataset contains 10 distinct classes of land cover, including:

Annual Crop
Forest
Herbaceous Vegetation
Highway
Industrial
Inland Water
Permanent Crop
Residential
River
Sea and Lake
Unlabelled
CNN model

The CNN model used in this repository is inspired by the VGG16 architecture. It consists of a series of convolutional layers, followed by pooling layers and fully connected layers. The final layer of the model outputs a vector of 10 probabilities, one for each class in the EuroSAT dataset.

Training the CNN model

To train the CNN model, you can use the following steps:

Clone this repository and install the required dependencies.
Download the EuroSAT dataset and unzip it into the data directory.
Run the train.py script.
This will train the CNN model on the EuroSAT dataset for 10 epochs. You can adjust the number of epochs by changing the epochs parameter in the train.py script.

Evaluating the CNN model

Once the CNN model has been trained, you can evaluate its performance on the EuroSAT test set by running the evaluate.py script. This will print the accuracy of the model on the test set.

Using the CNN model

Once the CNN model has been trained and evaluated, you can use it to classify new satellite images. To do this, you can use the predict.py script. This script takes a path to a satellite image as input and outputs a vector of 10 probabilities, one for each class in the EuroSAT dataset.

Example usage

To train the CNN model, run the following command:

python train.py
To evaluate the CNN model on the EuroSAT test set, run the following command:

python evaluate.py
To classify a new satellite image, run the following command:

python predict.py <path/to/image.jpg>
This will print the vector of 10 probabilities for the image. The class with the highest probability is the predicted class.

Conclusion

This repository provides a simple and easy-to-use way to train and evaluate a CNN model for satellite image classification. The code is well-documented and easy to understand
