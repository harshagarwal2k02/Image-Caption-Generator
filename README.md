# Image Captioning Generator

Welcome to the Image Captioning Generator project repository for the EE769 course project.

## Team Members:
- Harsh Agarwal <21B090007>
- Prankul Yadav <21D070050>
- Jayveer Singh Shikarwar <21D070033>

## Project Overview

This project focuses on generating captions for images using various encoder-decoder architectures. We have implemented multiple models with pretrained VGG-19 and ResNet-152 as encoders and LSTM, modified LSTM, and LSTM with attention as decoders. With these combinations, we've developed a total of 6 models. For a detailed overview, please refer to our [report](https://github.com/harshagarwal2k02/Image-Caption-Generator/blob/main/report.pdf).

## Getting Started

To run the code, follow these steps:

1. Install the required packages using the following command:
    ```
    pip install -r requirements.txt
    ```

2. Run the desired model using Jupyter Notebook or Google Colab. If using Google Colab, no installation is required.

## Repository Structure

- **models(https://github.com/harshagarwal2k02/Image-Caption-Generator/tree/6176af269ee14cceb71124613cff88338c796d68/models)**: Contains all the code files (.ipynb) for different models. Pre-presentation models are in the "pre_presentation" folder, while post-presentation models are in the main "models" folder.
- **pics(https://github.com/harshagarwal2k02/Image-Caption-Generator/tree/6176af269ee14cceb71124613cff88338c796d68/pics)**: Holds all the images used in the project.
- **test(https://github.com/harshagarwal2k02/Image-Caption-Generator/tree/6176af269ee14cceb71124613cff88338c796d68/test)**: Includes models that have been tested.

## How to Interpret Outputs

Each code file includes a `train()` function, which trains the model using cross-entropy loss and Adam optimizer for 10 epochs. During training, it prints the loss and perplexity on the training set and calculates BLEU and METEOR scores after validation. After training, you can observe the model's image captioning capabilities using the `generate_captions_for_random_image()` function, which takes the trained model as input and generates a caption for a random image from the validation set. Pre-run outputs are available for reference.
