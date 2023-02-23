# Identifying the edge of the optic cup and optic disc for Glaucoma using segmentation and fundus image classification via deep learning

## Table of Contents
1. [Overview](#overview)
2. [Getting Started](#getting-started)
    1. [Dependencies](#dependencies)
    2. [Models Used](#models)
    3. [Data Links](#data)
3. [Instruction to Run](#instruction)
4. [Sample Screen Shots](#sample)


## Overview <a name="overview"></a>
Human eye has a lot of diseases, here we will using some classification techniques on fundas images and .we need to distinguish between fundus diseases such as glaucoma, myopia, DR1, and maculopathy and normal images.here we will be using grad Cam as it highlights the region with makes biological senses and then we also use some segmentation techniques in gluacoma images and segment the optic cup and optic disc.we will use canny and dilation to get the edge over the optic cup and optic disc.


## Getting Started <a name="getting-started"></a>

### Dependencies <a name="dependencies"></a>
* Python 3.*
* Libraries: NumPy, Sklearn, Seaborn, Matplotlib, cv2, Keras, Tensorflow, tdpm, h5py,Skimage, Scipy, 
* Juypter

### Models Used <a name="models"></a>
we have few classification techniques like MobileNetV2,ResNet152,101 and 50V2, VGG16 also comapared these models. For segmentation we have pre-trained models like U-Net,U-Net++,W-Unet and ResUnet also comapared these models in terms of accuracy metric.
- *** All the code for gluacoma segmentation using U-Net is avaliable in [gluacoma](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/glucoma)
- *** All the code for gluacoma segmentation using other models is avaliable in [cnn](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/cnn)

### Data links<a name="data"></a>
- Model Link Drishti_GS: https://drive.google.com/drive/folders/14_FTu5JDokkWa4VKmOsm4GwjOJrWau33?usp=sharing
- Data set link for Gluacoma: https://drive.google.com/drive/folders/1S5KglW1s6m9D20WeGdC5hLfkr2_ZSoWq?usp=share_link
- Data set Link for Fundus Classification: https://www.kaggle.com/linchundan/fundusimage1000

## Instruction to Run<a name="instruction"></a>
### fundus classification 
* Download the data set from the link provide in data links and keep those data in the a folder where you will be executing yor project 
* Import the required libraries for the code and preprocess the data 
* Now train the model without fine-tuning and obtain the metrices 
* Now train the model with fine-tuning and obtain the metrices 
* Compare both the metrices to conclude with model work better
* Create a Grad-Cam function to generate the heatmaps
* Once the Heatmaps are generated test that on the testing images to final output that highlights the region with makes biological senses
* Reference : All the code for classification will be avaliable in [Eye](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/eye)

### Edge Detection 
* Download the model from the link provide in data links and keep those data in the a folder where you will be executing yor project 
* Import the required libraries for the code 
* Create the function for obtaining accuracy and loss for the model 
* Create the helper function to increase the brightness, hue, saturation, value and also code to shuffle instead of random shuffle
* Now load the data from the folder where you saved it
* Create a function for the segmentation model 
* Now prepare the data for our model injection
* Visualise  all the input data we have prepared 
* Create train and test set by combining datasets
* Preprocessing step for disc/ cup Segmentation and Perform CLAHE on each image
* Visualise  all the CLAHE data image after preprocessing
* create an helper function for callback and ReduceLROnPlateau
* Compile the model and then train it
* once training is done Visualise it on our dataset using canny and dilation for edge detection of cup and disc.
* Reference: All the code for gluacoma segmentation using U-Net is avaliable in [gluacoma](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/glucoma)
* Reference: All the code for gluacoma segmentation using other models is avaliable in [cnn](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/cnn)

## Sample Screen Shots] <a name="sample"></a>
