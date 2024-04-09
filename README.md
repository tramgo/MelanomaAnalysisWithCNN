
# Melanoma Detection using a Custom CNN with Keras+TensorFlow

## Project Overview

Melanoma, a deadly skin cancer, is curable if detected early. This project aims to develop a CNN-based model to accurately detect melanoma from dermatological images, potentially assisting dermatologists and reducing manual diagnosis efforts.

The dataset comprises 2357 images of various malignant and benign skin conditions from the International Skin Imaging Collaboration (ISIC). It includes a diverse set of diseases, with a slight dominance of melanoma and mole images.

## Data Understanding

Paths are defined for the training and test images. The dataset is sorted according to ISIC classifications, with nine classes represented.

## Dataset Creation

- The training and validation datasets are created from the training directory.
- Batch size is set to 32, and images are resized to 180x180 pixels.

## Dataset Visualization

- A visualization script is included to show one instance of each of the nine classes.

## Model Building & Training (Initial)

- A custom CNN model is created to detect the nine classes, with image rescaling as a part of the model.
- An appropriate optimizer and loss function are chosen.
- The model is trained for ~20 epochs, and the fit is assessed for evidence of overfitting or underfitting.

## Data Augmentation

- A data augmentation strategy is implemented to address any fitting issues.

## Model Building & Training (Post-Augmentation)

- The model creation process is repeated with data augmentation in place.
- The model is trained for ~20 additional epochs.
- The effectiveness of the augmentation strategy is evaluated.

## Class Distribution Analysis

- The class distribution in the training set is examined to identify the least and most represented classes.

## Handling Class Imbalances

- The Augmentor library is used to rectify class imbalances in the training dataset.

## Model Building & Training (Post-Class Imbalance Adjustment)

- A CNN model is created and trained for ~30 epochs on the balanced dataset.
- The model fit is evaluated to see if class imbalance issues have been resolved.

Each stage requires key accomplishments, such as setting up the data, creating and evaluating models, and addressing issues like overfitting and class imbalances.

## Conclusion

This project encapsulates the end-to-end process of developing a CNN model for melanoma detection, from data preparation to model evaluation, with an emphasis on addressing class imbalance and improving model performance.
