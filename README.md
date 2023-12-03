# American-Sign-Language-D.L.-Model
This repository contains the code for Joshua Wilbur and Amir Seidakhmetov's ECE 491 final project. This is a deep-learning model which can identify sign language gestures in images. All work was done in Google Colab before uploading.

# Model Specs Below:
The model is a fine-tuned VGG19 base model with ImageNet preloaded weights. 

Total trainable parameters: 9,614,365

Six layers were placed at the output of the VGG19 model for feature extraction

Three of these layers were fully connected (F.C.) layers

First layer (512 units): ReLU activation, 9,437,696 parameters

Second layer (256 units): ReLU activation, 131,328 parameters

The above two F.C. layers have L1 bias regularization, improved model convergence

The final layer has 29 units and softmax activation to classify the image into 1 of 29 categories

Batch normalization is used between layers to improve training efficiency

40% dropout used before the second F.C. layer to fight overfitting

Adam optimizer used with 0.0014 learning rate

Categorical cross-entropy loss function

