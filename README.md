# COVID Correct Hand Washing Prediction System

This project develops an image classification model to identify the 8 stages of proper handwashing technique as specified by WHO guidelines. 

## Data

The dataset consists of images of hands at various steps of handwashing - turning on tap, dispensing soap, lathering palms, scrubbing fingers etc. Images have been aggregated into 8 stage wise folders. Each contains approximately 300-500 images collected from multiple contributors.

## Model Pipeline

A convolutional neural network (CNN) is developed for classifying images into one of the 8 handwashing stages. The model code trains a CNN with convolutional layers for feature extraction, spatial max pooling, dropout regularisation, dense hidden layers and a softmax output layer.

## Training

The model is compiled with a categorical crossentropy loss function and rmsprop optimiser. Accuracy is monitored on validation set for regular evaluation. The CNN is trained for 20 epochs with a batch size of 32. Data augmentation techniques like rotation, zooming, horizontal flips are used to expand the training distribution.

## Evaluation

Model performance is analysed using confusion matrix, classification report and overall accuracy on the held out test set. These metrics convey model viability for deployment.
