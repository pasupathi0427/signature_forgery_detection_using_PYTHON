# Signature Forgery Detection with One-shot Learning

## Description

Conventional deep learning methods require large samples of data for a class in the classification process. One shot learning, being a method of meta learning, can perform classification tasks with one data point. Hence for the tasks like facial recognition, audio recognition, signature forgery verification this method of meta learning becomes more suitable at industrial level. For our project we performed signature forgery: identifying if a signature has been forged or otherwise.

## Main features

- Compare signatures and detect if they have been forged or not
- Can also work on new data without retraining
- Works with the accuracy of ~99%

## Tech Stack and concepts used

- Python
- Keras
- OpenCV
- Matplotlib
- Scikit-learn
- Convolution Neural Network
- Siamese Neural Network

## Thought behind the project

Using one-shot learning for signature forgery detection we can predict whether a signature has been forged or not using only one genuine signature for comparison without retraining the whole model. Also, one-shot learning models does not require huge datasets to train and can generalize very well.

## Setup

- Dowload the datasets and upload it the google drive and run the check_forgery.ipynb using google colab

- Download the model [signature_forgery_one_shot.h5](https://drive.google.com/file/d/1Y-JsSxrbGIiOPLcbUOw_YInZdXBYDSMB/view?usp=drive_link) and upload it in your Google Drive




## Results

| Model                                             | Training Set Accuracy | Validation Set Accuracy | Testing Set Accuracy |
| ------------------------------------------------- | --------------------- | ----------------------- | -------------------- |
| Basic CNN model                                   | 100 %                 | 88.14 %                 | 87.80 %              |
| CNN model with Regularization                     | 96.64 %               | 88.62 %                 | 88.53 %              |
| CNN model with Data Augmentation                  | 96.82 %               | 90.07 %                 | 88.78 %              |
| CNN model with Data Augmentation & Regularization | 97.38 %               | 90.31 %                 | 88.78 %              |
| VGG16 model                                       | 99.63%                | 94.43%                  | 93.90 %              |
| Siamese Network model                             | 99.88%                | 100%                    | 98.94 %              |
