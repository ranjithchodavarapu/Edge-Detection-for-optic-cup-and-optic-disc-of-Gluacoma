# Identifying the edge of the optic cup and optic disc for Glaucoma using segmentation and fundus image classification via deep learning

## Table of Contents
1. [Overview](#overview)
2. [Getting Started](#getting-started)
    1. [Dependencies](#dependencies)
    2. [Models Used](#models)
    3. [Data links] (#data)
3. [Instruction to Run](#instruction)

## Overview <a name="overview"></a>
Human eye has a lot of diseases, here we will using some classification techniques on fundas images and .we need to distinguish between fundus diseases such as glaucoma, myopia, DR1, and maculopathy and normal images.here we will be using grad Cam as it highlights the region with makes biological senses and then we also use some segmentation techniques in gluacoma images and segment the optic cup and optic disc.we will use canny and dilation to get the edge over the optic cup and optic disc.


## Getting Started <a name="getting-started"></a>

### Dependencies <a name="dependencies"></a>
* Python 3.*
* Libraries: NumPy, Sklearn, Seaborn, Matplotlib, cv2, Keras, Tensorflow, tdpm, h5py,Skimage, Scipy, 
* Juypter
* 
### Models Used <a name="models"></a>
we have few classification techniques like MobileNetV2,ResNet152,101 and 50V2, VGG16 also comapared these models. For segmentation we have pre-trained models like U-Net,U-Net++,W-Unet and ResUnet also comapared these models in terms of accuracy metric.
- *** All the code for classification will be avaliable in [Eye](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/eye)
- *** All the code for gluacoma segmentation using U-Net is avaliable in [gluacoma](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/glucoma)
- *** All the code for gluacoma segmentation using other models is avaliable in [cnn](https://github.com/ranjithchodavarapu/Edge-Detection-for-optic-cup-and-optic-disc-of-Gluacoma/tree/main/cnn)
### Data links<a name="data"></a>
- Model Link Drishti_GS: https://drive.google.com/drive/folders/14_FTu5JDokkWa4VKmOsm4GwjOJrWau33?usp=share_link
- Data set link: https://drive.google.com/drive/folders/14_FTu5JDokkWa4VKmOsm4GwjOJrWau33?usp=share_link


