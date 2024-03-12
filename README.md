## Melanoma Detection Assignment 

This repository is created as a part of the Melanoma Detection Assignment Module required for Melanoma Detection Assignment to build a CNN-based model that can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early, accounting for 75% of skin cancer deaths. A solution capable of evaluating images and alerting dermatologists about the presence of melanoma has the potential to reduce a significant amount of manual effort needed in diagnosis.

### Dataset Overview

The dataset consists of 2357 images of malignant and benign oncological diseases sourced from the International Skin Imaging Collaboration (ISIC). Images were categorized into 9 classes based on ISIC classification. The dataset includes the following classes:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

### Project Pipeline

1. **Data Reading/Data Understanding:** Define the path for train and test images.
   
2. **Dataset Creation:** Create train & validation datasets from the train directory with a batch size of 32. Resize images to 180x180.

3. **Dataset Visualization:** Visualize one instance of all nine classes present in the dataset.

4. **Model Building & Training:**
   - Create a CNN model to accurately detect the 9 classes. Rescale images to normalize pixel values between 0 and 1.
   - Choose an appropriate optimizer and loss function.
   - Train the model for approximately 20 epochs.
   - Write findings after model fit, checking for evidence of overfitting or underfitting.

5. **Data Augmentation:**
   - Choose an appropriate data augmentation strategy to resolve underfitting/overfitting.

6. **Model Building & Training on Augmented Data:**
   - Create a CNN model on augmented data.
   - Train the model for approximately 20 epochs.
   - Write findings after model fit to see if earlier issues are resolved.

7. **Class Distribution Analysis:**
   - Examine the current class distribution in the training dataset.
   - Identify the class with the least number of samples and the classes dominating the data.

8. **Handling Class Imbalances:**
   - Rectify class imbalances present in the training dataset with Augmentor library.

9. **Model Building & Training on Rectified Class Imbalance Data:**
   - Create a CNN model on rectified class imbalance data.
   - Train the model for approximately 30 epochs.


 The inferences and model results are shared below :
![Model Params](https://github.com/kanhu123mishra/Melanoma-Detection-Assignment/raw/main/model-stats.PNG)

![Model Accuracy](https://github.com/kanhu123mishra/Melanoma-Detection-Assignment/raw/main/model-params.PNG)



References :
https://learn.upgrad.com/course/4701/segment/46300/277670/845791/4239776
https://medium.com/deep-learning-turkey/google-colab-free-gpu-tutorial-e113627b9f5d
