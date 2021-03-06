## CNN-AlexNet-
CNN network AlexNet architecture explained with cat vs dog classifier example


# AlexNet architecture

  Layer (type)            |    Output Shape            | Param # |   
--------------------------|:--------------------------:|--------:|
conv2d_1 (Conv2D)         |   (None, 55, 55, 96)       |  34944  |  
batch_normalization_1     |(Batch (None, 55, 55, 96)   |   384   |     
activation_1 (Activation) |   (None, 55, 55, 96)       |    0    |    
max_pooling2d_1           | (None, 27, 27, 96)         |    0    |   
conv2d_2 (Conv2D)         |   (None, 27, 27, 256)      | 614656  | 
batch_normalization_2     | (None, 27, 27, 256)        |  1024   |  
activation_2 (Activation) |    (None, 27, 27, 256)     |    0    |  
max_pooling2d_2           | (None, 13, 13, 256)        |    0    |  
conv2d_3 (Conv2D)         |   (None, 13, 13, 384)      |  885120 | 
conv2d_4 (Conv2D)         |  (None, 13, 13, 384)       | 1327488 |
conv2d_5 (Conv2D)         |   (None, 13, 13, 256)      | 884992  |
batch_normalization_3     | (None, 13, 13, 256)        |  1024   | 
activation_3 (Activation) |   (None, 13, 13, 256)      |   0     | 
max_pooling2d_3           | (None, 6, 6, 256)          |   0     |
flatten_1 (Flatten)       |   (None, 9216)             |   0     |
dense_1 (Dense)           |   (None, 9216)             | 84943872|
batch_normalization_4     | (None, 9216)               |  36864  |
activation_4 (Activation) |   (None, 9216)             |  0      |
dense_2 (Dense)           |   (None, 4096)             | 37752832|
batch_normalization_5     | (None, 4096)               |  16384  |
activation_5 (Activation) |   (None, 4096)             |    0    |
dense_3 (Dense)           |   (None, 1)                |   4097  |
batch_normalization_6     | (None, 1)                  |    4    |
activation_6 (Activation) |   (None, 1)                |    0    |


### About the model
This model is built with AlexNet architecture on around 25000 Cat and Dog images. This model has a accuracy more than 72% on test set.

### About the dataset
This dataset is downloaded from kaggle weblsite. The data set can be downloaded from the link given in this repository file. This data set contains 2 classes 
Cat and Dog. This data set contain total of 25000 examples (including training ,validation and testing sets).

## preview of this data set
#### Cat
<img src="https://user-images.githubusercontent.com/61901749/87148566-40881b00-c2cc-11ea-9ddf-b9fca5b03845.jpg" width=350>         <img src="https://user-images.githubusercontent.com/61901749/87148571-4251de80-c2cc-11ea-9b7d-931c95151a72.jpg" width=350>
<img src="https://user-images.githubusercontent.com/61901749/87148572-42ea7500-c2cc-11ea-87cc-1e49ce68ce6d.jpg" width=350>         <img src="https://user-images.githubusercontent.com/61901749/87148574-43830b80-c2cc-11ea-85ba-1d4ecb4dd9e0.jpg" width=350>

#### Dog
<img src="https://user-images.githubusercontent.com/61901749/87149066-30bd0680-c2cd-11ea-8004-16209e292913.jpg" width=350>         <img src="https://user-images.githubusercontent.com/61901749/87149071-3286ca00-c2cd-11ea-998c-606afa00d1f3.jpg" width=350>
<img src="https://user-images.githubusercontent.com/61901749/87149075-331f6080-c2cd-11ea-91f3-2f7cda33fda8.jpg" width=350>         <img src="https://user-images.githubusercontent.com/61901749/87149079-33b7f700-c2cd-11ea-958e-3aff1e6e6ffc.jpg" width=350>


 ## MODEL ACCURACY : 72.80%
