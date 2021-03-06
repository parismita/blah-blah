# To contribute

The main file is cam.py, 
cifar.py contains the Neural Network Model, 
resize.py is for reducing the video size for faster training


Here's the Parameter List:

![Parameters](https://github.com/parismita/EyedBot/blob/master/ss.png)

The code :
* The model has 3 layers of convolution and pooling
* Dropout applied for Regularisation
* ReLu activation used
* binary_crossentropy loss function applied
* Optimization technique Adamax used (can use rmsprop too for best results)
* Euclidian Metric used for accuracy calculation

Dataset:
* Imagenet dataset used
* numpy train and test data is created in the file resize.py
* trainX dimension: (5760, 3, 70, 70) 
* trainY dimention: (5760,)
* sklearn used for randomization in file resize.py

Training:
* model.fit trains the model
* Validation set of 20% data taken 

Testing:
* 20% test data seperated via resize file
* done in cam.py
* Stored test prediction in file Trial.txt
