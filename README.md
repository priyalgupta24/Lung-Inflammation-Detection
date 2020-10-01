# Lung-Inflammation-Detection

## Introduction
Pneumonia is a life threatening lung inflammatory disease caused by viral or bacterial
infection of the lungs. Early diagnosis is vital for efficient treatment. When detecting
Lung Inflammation, CT scans are analyzed. The CT screening of millions of people puts
a huge burden on radiologists and manual detection may be faulty. Hence recent efforts
are to come up with an algorithm to automatically detect risks with professional accuracy.

## Dataset
We will be using the Kaggle dataset Chest X-Ray Images (Pneumonia). The dataset is
organized into 3 folders (train, test, val) and contains subfolders for each image category
(Pneumonia/Normal). There are over 5,000 X-Ray images (JPEG) and 2 categories
(Pneumonia/Normal).
The training set: Images we’re going to train the neural network on.
The validation set: Images we’re going to use to check if the model is underfitting or
overfitting.
The test set: These are images we’re going to use to check how good our neural network
is with data it has not seen before.
- 5216 images belonging to 2 classes in the training set.
- 16 images belonging to 2 classes in the validation set.
- 624 images belonging to 2 classes in the test set.

Preprocessing and data augmentation have been performed. For our train, validation
and test sets, we will zoom the image randomly by a factor of 0.2, Rescale pixel values to
0 to 1, randomly flip half the images horizontally and vertically, and apply shear based
transformations randomly.
We will run most models for 326 steps per epoch (number of batches per epoch) with
a batch size of 16.

## Plan Of Work
We have trained various models on our kaggle dataset like CNN, Resnet-50, VGG16, etc. For this purpose we have used kaggle notebooks which are attached along with the code. Then we compared and analysed their accuracies to determine the highest accuracy model.  
