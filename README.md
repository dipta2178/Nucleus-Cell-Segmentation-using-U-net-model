#CSE465 (Pattern Recognition and Neural Network) Project

Automatic segmentation of microscopy images is an important task in medical image processing and analysis. Nucleus detection is an important example of this task. Imagine speeding up research for almost every disease, from lung cancer and heart disease to rare disorders. The 2018 Data Science Bowl(https://www.kaggle.com/c/data-science-bowl-2018) offers our most ambitious mission yet: create an algorithm to automate nucleus detection. We’ve all seen people suffer from diseases like cancer, heart disease, chronic obstructive pulmonary disease, Alzheimer’s, and diabetes. Think how many lives would be transformed if cures came faster. By automating nucleus detection, you could help unlock cures faster from rare disorders to the common cold.

This is a typical instance segmentation problem. Two architectures which have been highly successful at this are U-Net and Mask-R-CNN. We used U-Net in this project.


Image Classification: Classify the main object category within an image.


Object Detection: Identify the object category and locate the position using a bounding box for every known object within an image.


Semantic Segmentation: Identify the object category of each pixel for every known object within an image. Labels are class-aware.


Instance Segmentation: Identify each object instance of each pixel for every known object within an image. Labels are instance-aware.


At first, we set some of the parameter values and load the training and test set images.
Next, we prepare the data in the form we want. To reduce the computational complexity we need to resize all the images. Then, we used Data augmentation technique. Because our dataset size is not enough for good prediction. Then we build our U-net model.


Activation function: Sigmoid
Optimizer: Adam
Loss function: Binary_crossentropy



