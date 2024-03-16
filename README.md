# Melanoma Skin Cancer Detection

## Abstract

To enhance the accuracy of skin cancer classification using images of skin lesions, I've created a customized CNN model. Melanoma, the deadliest form of skin cancer among over 200 types, demands swift and accurate diagnosis. Initial steps involve visual examination of skin lesions, often aided by dermatoscopic images. While these images alone yield 65-80% accuracy in diagnosing melanoma, combining them with expert visual assessment can raise accuracy to 75-84%. This project aims to automate this process using image processing techniques for precise skin cancer classification.

## Problem Statement
In a standard skin biopsy procedure, a dermatologist extracts a sample from a skin lesion and analyzes it using a microscope. However, this process typically spans over a week, from scheduling the appointment with the dermatologist to receiving the biopsy report.

Efforts are underway to significantly reduce this waiting period to just a few days through the implementation of a predictive model. This innovative approach employs Convolutional Neural Network (CNN) technology to categorize nine distinct types of skin cancer based on images of abnormal lesions. The potential outcome of minimizing this waiting time holds promise for a substantial positive impact on countless individuals.

## Motivation
The primary objective is to aid in the reduction of fatalities stemming from skin cancer. This initiative is propelled by a strong desire to leverage cutting-edge image classification technology for the benefit of public health. Remarkable advancements in computer vision, particularly in machine learning and deep learning, have rendered these methodologies applicable across various fields.

## Dataset
The dataset consists of 2239 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images.

### Sample image from Dataset

![sample image](https://github.com/chaitanyapss/Melanoma_Prediction/blob/main/download.png)

## CNN Architecture Design
To address the task of classifying skin cancer from images of skin lesions, I developed a customized Convolutional Neural Network (CNN) model aimed at achieving superior accuracy and performance in the classification process.

Rescaling Layer: This layer is designed to normalize the input data, transforming pixel values from the [0, 255] range to the [0, 1] range, ensuring consistency in data representation.
Convolutional Layer: Convolutional layers apply filters to input data, extracting features and passing them to subsequent layers. This process effectively condenses information within receptive fields, reducing image dimensions while consolidating relevant features.
Pooling Layer: Utilized to downsample feature maps, pooling layers aid in parameter reduction and computational efficiency within the network. By summarizing feature representations in specific regions, they contribute to streamlined processing.
Dropout Layer: Integrated to mitigate overfitting, dropout layers randomly deactivate input units during training, thereby enhancing model generalization by preventing reliance on specific features.
Flatten Layer: Responsible for converting multidimensional data into a one-dimensional array, the flatten layer prepares feature maps from convolutional layers for input into subsequent fully connected layers.
Dense Layer: Serving as a deeply connected neural network layer, dense layers ensure comprehensive interconnection between neurons, with each neuron receiving input from every neuron in the preceding layer.
Activation Function (ReLU): The rectified linear activation function (ReLU) is employed to introduce non-linearity into the network, facilitating faster learning and improved performance by overcoming issues such as vanishing gradients.
Activation Function (Softmax): Applied in the output layer of neural network models predicting multinomial probability distributions, the softmax function ensures output probabilities are within the range [0, 1], with their sum equating to one, facilitating probabilistic interpretation of results.

## References
Melanoma Skin Cancer from https://www.cancer.org/cancer/melanoma-skin-cancer/about/what-is-melanoma.html
