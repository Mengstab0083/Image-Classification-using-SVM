# MRI-Image-Classification-using-SVM
Image classification using Deep learning and Machine learning Techniques, The dataset selected for this work is an image dataset publicly available on Kaggle 1. The dataset
contains four classes i.e. mild demented, moderate demented, non demented and very mild demented. There are total 6400 magnetic resonance imaging (MRI) images.

## Project Structure

- `data_loader.py`: Contains the `load_dataset` function to load images and labels from a specified directory.
- `feature_extraction.py`: Implements the `preprocess_and_feature_extraction` function to extract features from images using HOG, VGG16, or a hybrid method.
- `classifier.py`: Includes the `train_svm_classifier` function to train an SVM classifier using the extracted features.
- `main.py`: The main script that ties everything together, processing command-line arguments, executing the feature extraction, training the classifier, and evaluating the results.

## Installation

To set up the environment and to run the scripts, follow these steps:

1. Install the required Python packages:

`pip install -r requirements.txt`

2. To run the main script, use the following command:

`python main.py --image_size 28 --technique hog`

or

`python main.py --image_size 224 --technique vgg`

or 

`python main.py --image_size 224 --technique hybrid`
