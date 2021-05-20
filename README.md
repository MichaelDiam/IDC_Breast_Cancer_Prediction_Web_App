# IDC Breast Cancer Prediction Web App

## Inspiration
Breast cancer is the most common form of cancer in women, and invasive ductal carcinoma (IDC) is the most common subtype of all breast cancers. Being able to accurately identify and categorize breast cancer subtypes is an important clinical task, and automated methods can be used to save time and reduce error. 

## Description
This project is a web app that uses Machine Learning & Convolutional Neural Networks (CNN) to predict if a carcinoma is malignant or benign. The app will be hosted by three different Python web frameworks Flask, Dash and Streamlit.

## Data
The original dataset is consisted of 162 whole mount slide images of Breast Cancer (BCa) specimens scanned at 40x. From that, 277,524 patches of size 50 x 50 were extracted (198,738 IDC negative and 78,786 IDC positive). The dataset can be found [here](https://www.kaggle.com/paultimothymooney/breast-histopathology-images):

## File Structure
* datasets
  * single_prediction - slide images for testing single prediction
  * test_set - test set
  * training_set - training set 
  * validation_set - validation set 
    
    note: folders '0' and '1' inside the three above folders contain benign and malignant slide images respectively
    
* IDC Breast Cancer Prediction with CNN.ipynb 
  * Loading the dataset of slide images
  * Image preprocessing & feature scaling
  * Designing and Building the same CNN model with both Keras and Pytorch libraries
  * Training the models
  * Testing the models
  * Evaluating the results
  * Choosing the final model
  * Testing on a signle prediction

* model.pt
  * The saved trained model to be used from the web app
