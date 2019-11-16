# cloud-segmentation
Kaggle Competition on Cloud Segmentation [Click here for detail](https://www.kaggle.com/c/understanding_cloud_organization/)

## Overview
In this challenge, we are building a model to classify cloud organization patterns from satellite images. There are four classes of clouds used here: **fish, flower, gravel, sugar**

## Comments
1. I used both **FPN** and **UNet** architecture for testing as they are evaluated to be better than other segmentation neural nets I tried (PSPNet, Linknet)
2. Attempted to try different combinations of backbones (Resnet34, Resnet50, EfficientNetB2), and decided to stick with **EfficientNetB2** as it performed consistently well for this particular dataset.
3. Tried to apply Data Generator so as to real-time augment input training images in streams. 

Overall managed to achieve 0.6579 (top 30%) for my first try on Kaggle despite having a fairly short training runway (2 weeks prior to submission). Further implementation details can be found in my Jupyter notebook (.ipnyb) file. 
