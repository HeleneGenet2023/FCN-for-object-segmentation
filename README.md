# FCN-for-semantic-segmentation
FCN usage for semantic segmentation on a highway dataset

## Overview

The following script performs image segmentation using a Fully Convolutional Network (FCN) built upon the VGG16 architecture. The FCN is trained to segment objects from the background in input images. This script includes functions to load data, preprocess groundtruth data, build the FCN model, visualize predictions, and create a video from the segmentation outputs.

![Segmentation Output](segmentation_output.gif)


## Dataset

The script is designed to work with data from the ChangeDetection.net (CDnet) 2012 dataset, specifically the highway sequence. You can obtain the dataset from the [ChangeDetection.net website](http://changedetection.net/)


## Prerequisites

Before you begin, ensure you have the following requirements:

## Python version
- Python 3.6 or above

## Packages
- os
- Numpy
- Matplotlib
- Scikit-Learn
- Tensorflow (2.x or later)
- Opencv-pytho

You can run the following command to install these packages:
pip install numpy matplotlib scikit-learn tensorflow opencv-python-headless

## Using the Image Segmentation Script

To use the image segmentation script, follow these steps:
1. Place your input images in a folder named 'input' and your ground truth data in a folder named 'groundtruth' in the same directory as the script
2. Run the script using a Python interpreter
3. The script will split the data into training, validation, and test data, and then train the model using the training data
4. After training, the script will evaluate the model using the test data, and then visualize some predictions using the 'visualize_predictions' function.
5. A video showing the segmentation results will be created and saved as 'segmentation_ouput.mp4' in the script's directory.
  
The main functions in the script are:
- 'load_data(data_path, is_groundtruth=False): Loads the data from the specified path. If is_groundtruth is True, the function expects grayscale images as ground truth data.
preprocess_groundtruth_data(data): Preprocesses the ground truth data by thresholding the pixel values.
- build_model(input_shape=(None, None, 3)): Builds the neural network model.
visualize_predictions(X_test, y_test, y_pred): Visualizes some predictions alongside the ground truth and input images.
- create_video(X_test, y_pred, output_path='segmentation_output.mp4', frame_size=(256, 256), frame_rate=10.0): Creates a video showing the segmentation results.

## Contact

You can reach me at helene.genet@polymtl.ca


