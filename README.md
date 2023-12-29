# Are-Pandas-more-like-Cats-or-like-Dogs-?
The project, titled "Are Pandas more like Cats or like Dogs?" involves the development of image classifiers using Convolutional Neural Networks (CNNs) to classify images of Pandas, Cats, and Dogs. The project is divided into three main parts: Initial Reorganization of the data, Panda-vs-Dog Classifier, and Panda-vs-Cat Classifier.

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
