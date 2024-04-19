# Image-Captioning-Generator

Repository for EE769 course project

Team Members :
-Harsh Agarwal<21B090007>
-Prankul Yadav<21D070050>
-Jayveer Singh Shikarwar<21D070033>

# Project Overview

In this project we made multiple models for Image Caption Generation. The models we made are in encoder-decoder architecture. The encoders used are pretrained VGG-19 Net and pretrained ResNet-152.The decoders used are LSTM, LSTM with slight modifications, LSTM with attention. Therefore, with 2 encoders and 3 decoders, we had made 6 models. For more information, please see the [report][https://github.com/harshagarwal2k02/Image-Caption-Generator/blob/main/report.pdf]

# Steps to run the code

1:Install the required packages using the command

`pip install -r requirements.txt`

2:Run the required model using jupyter notebook or google collab (If it is collab, then installation is not required).

# Repository Structure

All the codes are in [model](model) folder,models made before presentation(with BLEU score) are in "pre_presentation" folder and the ones made after (with METEOR score) are in the models folder.
All the images are in [pics](pics) folder.The codes include pre-saved outputs generated from prior runs.There are 6 codes files/ .ipynb files in models,each with a different encoder decoder pair according to the name of the file.
We used 2 encoders(VGG19 ,ResNet152) and 3 decoders(LSTM,LSTMmodified,LSTM_with_attention). The models that are test ran are in [test](test) folder.

# Interpretation of outputs

In each of the codes we wrote a similar train() function which trains the model using cross entropy loss and adam optimiser for 10 epochs,this function prints the loss and perplexity while training(on the train set) and also prints BLEU and METEOR scores after validation(using a validation set) after each epoch.After training the model we can observe the models image captioning capabilities using the function generate_captions_for_random_imag() which takes in the trained model as input and prints one random image(from validation set) and prints its generated caption when we send that image as input to our model.Our code has pre ran outputs for reference.
