# Animal Image Classification with CNNs

![Python](https://img.shields.io/badge/Python-blue?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-orange?logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-red?logo=keras&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-blue?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-blueviolet?logo=matplotlib&logoColor=white)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-lightblue?logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/ashishsaxena2209/animal-image-datasetdog-cat-and-panda)

## Abstract
The Animal Image Classification with CNNs project explores the use of Convolutional Neural Networks (CNNs) to classify images of Pandas, Cats, and Dogs. The primary goal was to determine whether pandas are more similar to cats or dogs through two classifiers: Panda-vs-Dog and Panda-vs-Cat. Using a Kaggle dataset with 1,000 images for each class, models were developed with incremental improvements, including dropout, regularization, and data augmentation. The Panda-vs-Dog classifier achieved a maximum accuracy of 96.0%, while the Panda-vs-Cat classifier achieved 95.5%. The project demonstrates the effectiveness of CNNs and highlights potential improvements using advanced architectures like VGG16.

## Animal Image Dataset (Dog, Cat, and Panda)

This repository provides access to a Kaggle dataset of animal images, featuring three classes: Dog, Cat, and Panda.

### Dataset Overview

- **Source**: [Kaggle - Animal Image Dataset (Dog, Cat, and Panda)](https://www.kaggle.com/datasets/ashishsaxena2209/animal-image-datasetdog-cat-and-panda)
- **Categories**:
  - Dog
  - Cat
  - Panda
- **Format**: The dataset consists of image files organized into respective category folders.

## Part I: Initial Reorganization of the Data

* Obtained a Kaggle dataset containing images of Pandas, Cats, and Dogs (1000 each).
* Used Colab to download and unzip the dataset.
* Reorganized the data into the required directory structure.

## Part II: Panda-vs-Dog Classifier
#### II.0 Creation of TF Datasets:

* Created TensorFlow Dataset objects for training, validation, and testing for the Panda-vs-Dog classification.
* Removed cat subdirectories from the datasets.

#### II.1 Preliminary CNN Model (pvdm1):

* Developed a simple CNN model without using dropout, regularization, or data augmentation.
* Achieved a test accuracy of 93.5%.

#### II.2 Improved CNN Model (pvdm2):

* Developed a second CNN model with dropout for improved performance.
* Achieved a test accuracy of 95.0%.

#### II.3 CNN Model with Data Augmentation (pvdm3):

* Developed a third CNN model using data augmentation during training.
* Achieved a test accuracy of 96.0%.

## Part III: Panda-vs-Cat Classifier

* Created a new directory to avoid conflicts with Part II.
* Removed dog datasets from the subdirectories.

#### III.1 Preliminary CNN Model (pvcm1):

* Developed a simple CNN model without dropout, regularization, or data augmentation for Panda-vs-Cat classification.
* Achieved a test accuracy of 91.0%.

#### III.2 Improved CNN Model (pvcm2):

* Developed a second CNN model with parameter regularization and dropout for improved performance.
* Achieved a test accuracy of 95.0%.

#### III.3 CNN Model with Data Augmentation (pvcm3):

* Developed a third CNN model using data augmentation for Panda-vs-Cat classification.
* Achieved a test accuracy of 95.5%.

## Conclusions:

* Employed callbacks, L2 regularization, and dropout to improve model performance.
* Data augmentation significantly improved model accuracy.
* Acknowledged the challenge of achieving high accuracy in the Panda-vs-Cat classification.
* Proposed the use of VGG16 architecture for further improvement.
* All models outperformed random classifiers on the test set.
