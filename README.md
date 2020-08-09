# Similar Image Finder

This model will find the n similar images from the training dataset of the input image. It leverages the feature extraction of pre-trained of resnet50
and KNN algorithm to find similar images.



## Libraries:

Keras,sklearn,skimage


## Workflow:

1. At first, pretrained resnet50 will be used to extract features of images.We downloaded only the feature extraction layer of resnet50 and paased all training images through it.

2. After passing it from resnet50 , we have flattened it and fitted it through knn where we used cosine distance and number of neighbours will depend on user input.

3. test image will go to resnet50 and then it will get nearest neighbours from the previously fitted knn and the similar image will be stored in output folder.




## folder strucutre:

Similar_image.py: It containes the core code. It needs to be invoked to get the similar images. It will ask for how many similar image to be fetced as input.

data: In this folder training data will reside in train folder. Query image will reside in test folder(you can keep as many as you want).

output: this folder will automatically be created results.

Other files contains various utility functions that will be used in core program file.


## Results:



