## in this repo im inserting the alex net paper that was published in 2012 and the code implmentation on cifar10 dataset 

![imagenet-6](https://user-images.githubusercontent.com/92921252/231774782-0e86ae45-6b29-42dc-9cae-52f9dec10b1a.png)


The architecture of AlexNet consists of eight layers: five convolutional layers followed by three fully connected layers. Here's a brief overview of each layer:
1.	Input layer: The network takes as input an RGB image of size 224x224x3.
2.	Convolutional layer (C1): The first convolutional layer has 96 filters of size 11x11 with a stride of 4. The filters are applied to the input image to produce 96 feature maps of size 55x55x96. The activation function used is the rectified linear unit (ReLU).
3.	Max pooling layer (S2): The output of the first convolutional layer is fed into a max pooling layer with a pool size of 3x3 and a stride of 2. This reduces the size of the feature maps to 27x27x96.
4.	Convolutional layer (C3): The second convolutional layer has 256 filters of size 5x5 with a stride of 1. The filters are applied to the output of the first max pooling layer to produce 256 feature maps of size 27x27x256. The activation function used is ReLU.
5.	Max pooling layer (S4): The output of the second convolutional layer is fed into a max pooling layer with a pool size of 3x3 and a stride of 2. This reduces the size of the feature maps to 13x13x256.
6.	Convolutional layer (C5): The third convolutional layer has 384 filters of size 3x3 with a stride of 1. The filters are applied to the output of the second max pooling layer to produce 384 feature maps of size 13x13x384. The activation function used is ReLU.
7.	Convolutional layer (C6): The fourth convolutional layer has 384 filters of size 3x3 with a stride of 1. The filters are applied to the output of the third convolutional layer to produce 384 feature maps of size 13x13x384. The activation function used is ReLU.
8.	Convolutional layer (C7): The fifth convolutional layer has 256 filters of size 3x3 with a stride of 1. The filters are applied to the output of the fourth convolutional layer to produce 256 feature maps of size 13x13x256. The activation function used is ReLU.
9.	Max pooling layer (S8): The output of the fifth convolutional layer is fed into a max pooling layer with a pool size of 3x3 and a stride of 2. This reduces the size of the feature maps to 6x6x256.
10.	Fully connected layer (F9): The output of the fifth max pooling layer is flattened into a vector of length 6x6x256=9216, which is fed into a fully connected layer with 4096 neurons. The activation function used is ReLU.
11.	Fully connected layer (F10): The output of the first fully connected layer is fed into a second fully connected layer with 4096 neurons. The activation function used is ReLU.
12.	Output layer (F11): The output of the second fully connected layer is fed into an output layer

![arch](https://user-images.githubusercontent.com/92921252/231774901-b4734e6c-1a4d-4110-bdbd-cb85d3c380fb.jpg)
