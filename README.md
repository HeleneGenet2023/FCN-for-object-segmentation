# FCN-for-semantic-segmentation
FCN usage for semantic segmentation on a highway dataset

## Overview

The following script performs image segmentation using a Fully Convolutional Network (FCN) built upon the VGG16 architecture. The FCN is trained to segment objects from the background in input images. This script includes functions to load data, preprocess groundtruth data, build the FCN model, visualize predictions, and create a video from the segmentation outputs.

## Requirements

Here are the needed packages to run the script: 
  -os
  -Numpy
  -Matplotlib
  -Scikit-Learn
  -Tensorflow (2.x or later)
  -Opencv-python

You can run the following command to install these packages:
pip install numpy matplotlib scikit-learn tensorflow opencv-python-headless


  
## Output
The script will output the following:
  -Test loss: Printed in the console.
  -Viasualizations: Displayed using matplotlib
  -Video: A video showing the segmentation output saved as 'segmentation_output.mp4' in the script<s directory.
