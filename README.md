# Deep Learning for Medical Image Classification

This repository contains the code for training a convolutional neural network (CNN) on a dataset of medical images for the purpose of binary classification. The model is trained to distinguish between normal and abnormal images.

## Project Overview

The project consists of several stages:

1. Data Preparation: Images are loaded from two folders, 'abnormal' and 'normal', corresponding to the two classes for classification. The dataset is split into training and validation sets.

2. Model Training: The model architecture is based on a pre-trained ResNet50 model, with the last layer modified to output two classes. The model is trained using Cross-Entropy Loss and the Adam optimizer.

3. Evaluation: The model's performance is evaluated on the validation set, with metrics such as accuracy, precision, recall, and F1-score being calculated.

4. Visualization: Grad-CAM is used to visualize which parts of the images the model focuses on when making a prediction.

## Requirements

To install the required libraries, run:

pip install pytorch-gradcam
pip install opencv-python


## Usage

To run the code, simply execute the `AbcessDetection.ipybn` script:

This will train the model on the data in the 'normal' and 'abnormal' folders and save the best model as 'best_model.pth'. The Grad-CAM visualizations will be saved as 'gradcam.jpg' and 'gradcam_pp.jpg'.

## Contributing

Pretrained Weights Come From My friend Model on Project Simmilar to this Project

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
