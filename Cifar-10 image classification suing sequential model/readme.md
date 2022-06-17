What is CIFAR-10 ?

CIFAR-10 consists of 10 classes, i.e., airplanes, cars, birds, cats, deer, dogs, frogs, horses, ships, and trucks.

Key Features of CIFAR-10:

 👉   10,000 test images, 1000 images per class. Test images are randomly-selected images from each class.

 👉   50,000 training images, 5000 images per class. The rest of images (minus the test images from total images) are comprised of training images. However, some training images may contain more images in one class.

 👉   The classes in the dataset are entirely mutually exclusive.

 👉   CIFAR-10 consists of 60,000 32 X 32 images (low resolution). They are mostly used in Convolutional Neural Network (CNN) models.

Here in this program i have build 2 python files, one for model creation and training and other for prediction.

Objective of the program is to find the corract class of image which is deer. 

# to run 
first execute command in Cifar_10_classification_model_building_and_saving.ipynb file 

# now you have saed .h5 file so you dont need to run model incase of same network structue just load .h5 file similar to second file
to load model run file : Model_accuracy,_Loading_model_and_Prediction.ipynb
## in above file i have loaded the model, predict the image class and find the accuracy of model
