# CrackDetection
Dataset
The dataset is available on Kaggle under the heading of surface crack detection dataset.
The data is collected from various METU Campus Buildings. The dataset is divided into two 
as negative and positive crack images for image classification. Each class has 20,000 images 
with a total of 40,000 images with 227 x 227 pixels with RGB channels.
Model
The image data is used without any resizing. While random rotation, cut-out and flipping
augmentation is used for improving the size of data and avoiding any overfitting by introducing 
noised data.
Efficientnet-B0 is used for the classification task. Transfer learning method is used for an 
optimal training the backbone of the model is freeze. And then a hand engineered fully 
connected layers are added. Pytorch framework is used for training and cross-validation.
AdamW optimizer coupled with CosineAnnealingLR learning rate scheduler is used for 
weights updating.
Mini batch methodology is used for training with 64 batch size as I was using Kaggle notebook 
so there is plenty of GPU Ram is available.
Holdout cross validation method is used for tracking the efficiency and avoiding any flaws in 
model training.
Application
Model can be used for disaster management and avoiding harm to lives during any natural
incident. It can also be used to avoid any part failure in machine learning
