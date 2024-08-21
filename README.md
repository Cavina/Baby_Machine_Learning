# Baby Monitor with Face Detection and Machine Learning

## Overview

This project is the machine learning portion of the embedded baby monitor project. It detects if a baby is face up or face down using different machine learning classifiers. The project encompasses data preparation, model training, and evaluation phases.
This project was meant to be proof of concept, and it succeeded. This project has been most useful as insight to beginner machine learning enthusiasts that are learning how to create their own dataset locally, prepare and analyze the data, as well as 
evaluate machine learning models and output.

## Features

- **Image Processing**: Processes and classifies images of the baby to determine orientation.
- **Data Preparation**: Organizes and labels images as face up or face down.
- **Model Training**: Trains machine learning models on the prepared dataset.
- **Model Evaluation**: Assesses model performance using accuracy metrics and confusion matrices.
- **Embedded Implementation**: Models are designed for real-time classification on embedded systems.

## Dataset

The dataset includes images of a baby labeled as either "FaceUp" or "FaceDown". The images should be organized in the following directory structure:

- `./DataSet/`
  - `FaceUp/`
    - `image1.jpg`
    - `image2.jpg`
    - `...`
  - `FaceDown/`
    - `image1.jpg`
    - `image2.jpg`
    - `...`
   
      
## Implementation

### Data Preparation

Images are loaded from local storage, resized, and labeled as either face up or face down. The prepared dataset is saved and loaded for training purposes.

### Model Training

Two types of classifiers are used in this project:

- **Nearest Centroid Classifier**: This classifier is trained and evaluated for detecting the baby's orientation.
- **Multilayer Perceptron (MLP) Classifier**: This neural network model is trained with various hyperparameters to find the optimal configuration for classification.

### Model Evaluation

The performance of the trained models is evaluated using accuracy scores and confusion matrices to determine their effectiveness in classifying the baby's orientation.

## Usage

- **Data Preparation**: Organize your images in the specified directory structure and run the data preparation script.
- **Model Training**: Train the machine learning models using the provided training scripts.
- **Model Evaluation**: Evaluate the models' performance and select the best-performing one.
- **Deployment**: Use the trained model for real-time classification on your embedded system.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

Thanks to the developers of the libraries and tools used in this project: OpenCV, Scikit-learn, and Matplotlib.

