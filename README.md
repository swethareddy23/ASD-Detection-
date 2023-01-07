# Autism Spectrum Disorder Detection 
## Introduction
* Autism spectrum disorder (ASD) is a neurological and developmental
disorder that affects how people interact with others, communicate, learn,
and behave.</br>
* Autism is known as a “spectrum” disorder because there is wide variation
in the type and severity of symptoms people experience.
## Objective
Design a deep learning based model architecture to predict if a child has
ASD or NOT, based on the Facial Expression.

## Dataset
>[Link to Dataset](https://www.kaggle.com/datasets/cihan063/autism-image-data)</br>
The dataset is taken from Kaggle which contains 2930 facial images of children
in the age group of 3-9 years in two subfolders Autistic and Non-Autistic.

#### Preview of Dataset
* Autistic Images from Dataset</br>
<img src= https://github.com/swethareddy23/Autism-Spectrum-Disorder-Detection/blob/main/asd/autistic.png width='400' height='250' /></br>

* Non-Autistic Images from dataset</br>
<img src= https://github.com/swethareddy23/Autism-Spectrum-Disorder-Detection/blob/main/asd/non_autistic.png width='400' height='250' /></br>

## Preprocessing: 
The purpose of the data preprocessing was to clean and crop
the images. Because the data were collected from Internet resources by Piosenka, they had to be preprocessed before they could be used to train the deep
learning model. The dataset creator automatically cropped the face from the
original image. Then, the dataset was split into 2,530 images for training, 200
for validation, and 200 for testing. To scaling, the normalization method was applied; the dataset was rescaling the parameters of all the images from the pixel
values [0, 255] to [0, 1].


## Training
#### Transfer Learning
The idea behind transfer learning is that a neural network that has been trained on a large dataset can apply its knowledge to a dataset it has never seen before.</br>
That's why it's called transfer learning because we transfer the learning of an existing model to a new dataset.
##### Challenges:
* Deep learning methods are data-hungry
* Greater than 50K data items needed for training
* The distributions of the source and target data must be the same.
* Labeled data in the target domain may be limited
* This problem is typically addressed with transfer learning
####  Model 1: Inception V3
* Inception V3 is a Deep Learning model based on Convolutional Neural
Networks, which is used for Image Classification.
* It is a version of the network already trained on more than a million images
from the ImageNet database.
* Inception-v3 is a CNN model that is 48 layers deep. This model consists of
two parts:
  *  1. Feature extraction part with a convolutional neural network.</br>
 * 2. Classification part with fully-connected and logistic layers.</br>
#### Model 2: ResNet 50
#### Model 3: VGG-19
