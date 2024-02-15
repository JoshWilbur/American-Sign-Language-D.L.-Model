# American-Sign-Language-D.L.-Model
This repository contains the code for Joshua Wilbur and Amir Seidakhmetov's ECE 491 final project. This is a deep-learning model which can identify sign language gestures in images. The model is 96% accurate during training and 77% accurate in testing. All work was done in Google Colab before uploading.

# Datasets
Two datasets were used for this model. The training dataset contains 7000-8000 images for each hand gesture. Twenty-nine classes of images are contained in this dataset. Since the validation data subset is small, an 80/20 split of the images was done to create the training and validation image generators. Training images were preprocessed using shear and zoom to help improve model generalization. The testing dataset is much smaller, with only thirty images for each of the twenty-nine classes. This is alright as this dataset was only used to see how accurate the model was in novel situations. Both datasets are linked below.

Training: https://www.kaggle.com/datasets/debashishsau/aslamerican-sign-language-aplhabet-dataset/data

Testing: https://www.kaggle.com/datasets/danrasband/asl-alphabet-test/data

# Model Archetecture:
Our model was a fine tuned VGG19 model. We placed six layers at the output of the VGG19 model for feature extraction. More details on the archetecture of the model can be found in the report uploaded to the repository.
