# Melanoma_Detection_Assignment

## Problem Statement:
- To build a CNN-based model that can accurately detect melanoma.
- Melanoma is a type of cancer that can be deadly if not detected early.
- It accounts for 75% of skin cancer deaths.
- A solution that can evaluate images and alert dermatologists about the presence of melanoma can potentially reduce the manual effort needed in diagnosis.

## Objective:
To build a Convolutional Neural Network for multiclass classification that can accurately detect melanoma.

## Dataset:
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed by the International Skin Imaging Collaboration (ISIC). 
All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, except melanomas and moles, whose images are slightly dominant.
* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion

## General steps that have been taken:
* Data Loading through Google Drive
* Initial Model Building
* Training the Model against this dataset
* Building an augmented model
* Training the augmented model
* Countering Class Imbalance with Augmentor
* Building the final model
* Training the final model

## How to execute the notebook?
- We need to upload the code into Google Colab and make sure that this is run on a GPU for faster processing.
- Please make sure that Google Colab has access to the dataset in the Google Drive directory mentioned in the code so that it can be accessed and mounted to start training the model.
- Furthermore, it is recommended to run this through a GPU as a CPU will take a lot of time. With that in mind, please make sure that there are enough computing units to ensure that we can run this through a GPU.

## Conclusions Drawn:
- Models built had very low training and validation accuracy due to class imbalance.
- The above was proven after augmentation was implemented through the [Augmentor](https://augmentor.readthedocs.io/en/master/) library.
- Models were further stabilized with a lower learning rate, to bring about stable convergence, reduce overfitting as much as possible and minimize oscillations
