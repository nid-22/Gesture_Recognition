# Smart TV Gesture Recognition Project
### Introduction

This project is a part  IIITB and Upgrad course, focusing on developing a feature for smart televisions. The goal is to enable smart TVs to recognize five different user gestures, allowing users to control the TV without a remote. This system is built using a 3D Convolutional Network (Conv3D), capable of processing and understanding the spatial-temporal patterns in video sequences of gestures.

### Problem Statement

 This project addresses the need of recognizing gestures performed by the user to control TV operations, using a sequence of RGB images processed by a Conv3D model.
 
### Dataset

The dataset comprises video sequences, each representing a specific gesture performed by the user. Each video is a sequence of 30 RGB frames with a resolution of 100x100 pixels, resulting in a 4-D tensor input shape for the Conv3D model.

### Model Architecture

The model utilizes a 3D Convolutional Network to process the video inputs. The key components of our architecture include:

    Conv3D Layers: To extract spatial-temporal features from the video sequence.
    Activation Functions: ReLU, used after each Conv3D layer for introducing non-linearity.
    Pooling Layers: MaxPooling3D, to reduce dimensionality and extract dominant features.
    Fully Connected Layers: To classify the extracted features into one of the five gestures.
    Output Layer: A softmax activation function to output the probability distribution over the five classes.

