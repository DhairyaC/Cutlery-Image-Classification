## Overview
Image classification using Machine Learning has many useful applications for daily tasks and has the potential to make our lives easier. Machine Learning programs aim to learn from images to find object patterns that make them recognizable. For example, we tend to recognize a fork because it has a handle, a neck and four points. Therefore, ML and Image classification should identify those patterns in a picture to classify it as a fork.

## Goal
I'm going to explore the application of data manipulation, transfer learning and a custom deep neural network to a cutlery image dataset to find the model with the best image classification performance for four categories - cup, knife, fork, spoon.

## Objectives
1. Take 100 images per class with at least 3 classes using my phone/camera. Display 5 examples from each class.
2. Split the images into a training set, a validation set, and a test set.
3. Build the input pipeline, including the appropriate preprocessing operations, and add data augmentation.
4. Fine-tune a pretrained Xception model on this dataset (the one I created in part 3). Report classification accuracy and give a few examples of correct/incorrect classification (show a few images that were correctly/incorrectly classified).
5. Train a deep neural network from scratch (without pretraining) that contains convolutional layers on this dataset (the one I created in part 3). Report classification accuracy and give a few examples of correct/incorrect classification (show a few images that were correctly/incorrectly classified).

## Techniques/Models
1. Techniques:
   - Keras image preprocessing
   - Data augmentation
   - Dataset prefetching
   - Reusing weights of neural network
   - Hyperparameter tuning
   - Model optimization
2. Models:
   - Xception model
   - ImageNet model
   - Custom Deep Neural Network
   
## Findings
1. The main difference observed when I computed the evaluation criteria between the fine-tuned pretrained model and the custom model developed from scratch is that the fine-tuned model gave higher accuracy for similar epochs compared to the custom model developed from scratch.
2. After 8 epochs, we see that there is no change in the accuracy for the custom model developed from scratch, thus either parameter fine-tuning is required or some change in the custom model architecture is required.
