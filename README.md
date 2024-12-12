# Machine Learning Final
# Predicting Pneumonia with MONAI and Multiple DenseNets

## Background and Motivation 
Pneumonia is an infection that causes inflammation in one of or both of the air sacs in the lungs. It leads to fluid or pus building up in the lungs making it difficult to breath and get air into the bloodstream. It is one of the leading causes of dealth in the United States, and was responsible for the dealth of 2.5 million people in 2019.

Traditionally, pneumonia is diagnosed by doctors analyzing chest X-rays of patients exhibiting symptoms. However, artificial intelligence (AI) offers the potential to simplify this process and reduce the risk of human error. By leveraging machine learning, AI can be trained to accurately predict whether chest X-rays indicate the presence of pneumonia, providing a reliable and efficient tool for diagnosis.

This AI model uses MONAI and different DenseNets to train on chest X-ray images to classify pneumonia, identifying whether a given X-ray shows signs of pneumonia or not, based on learned patterns from labeled training data. The images used are from MedMNIST's PneumoniaMNIST data set.

![Alt text](./results_images/normal_pneumonia_xray.png)

## Previous Studies Done
A previous study done by Anthony Novokshanov at Research Archive of Rising scholars examined the PnemoniaMNIST data set and was able to predict pneumonia with an accuracy of 91%. 
This was achieved by a seven layer convolutional neural network (CNN) with rectified linear unit (ReLU) functions that was created with PyTorch libraries and trained on a 15 epoch loop.

Our goal here is to exceed this accuracy through the use of DenseNets and training on a 100 epoch loop

https://www.researchgate.net/publication/352496130_Using_Explainable_Artificial_Intelligence_to_Locate_Pneumonia 

## Goal
The goal is to develop a highly effective model for predicting pneumonia from chest X-rays. Through the use of MONAI's DenseNet models, we aim to surpass the 91% accuracy achieved by Anthony Novokshanov. Additionally, this approach will allow us to compare the performance of different DenseNet variants (121, 169, 201, 264) and identify the most effective model.

## Methods 
### Dataset 
As previously mentioned, the dataset used in this model is MedMNIST's PneumoniaMNIST. 
It is a binary-class data set containing a total 5,856 sample chest x-rays. 
This is split into 4,708 training samples, 524 validation samples, and 624 test samples



