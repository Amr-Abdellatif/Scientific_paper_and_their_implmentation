## LeNet

LeNet, also known as LeNet-5, is a convolutional neural network architecture that was developed by Yann LeCun, Leon Bottou, Yoshua Bengio, and Patrick Haffner in the 1990s. 

It was one of the first successful models to demonstrate the power of convolutional neural networks in computer vision tasks.

![lenet5](https://user-images.githubusercontent.com/92921252/231776413-7486862c-ebad-44d3-a091-da4649ce9a15.png)

LeNet consists of seven layers: the input layer, two convolutional layers, two subsampling (pooling) layers, and two fully connected layers. The architecture takes as input a grayscale image of size 32x32 pixels.

The first layer is a convolutional layer that applies six 5x5 filters to the input image, producing six output feature maps. The second layer is a subsampling layer that reduces the spatial dimensions of each feature map by taking the maximum value in each 2x2 region, resulting in six 14x14 feature maps.
The third and fourth layers repeat the same process, with the third layer consisting of 16 5x5 filters applied to the six 14x14 feature maps, and the fourth layer consisting of subsampling to produce 16 5x5 feature maps.

The fifth and sixth layers are fully connected layers, each with 120 neurons, followed by a seventh and final fully connected layer with 10 neurons, representing the 10 possible classes in the MNIST dataset (handwritten digits).


The LeNet architecture has been widely used in handwritten digit recognition, but can also be applied to other computer vision tasks with small-sized images. It served as a foundation for many later models, such as AlexNet, VGGNet, and ResNet, that have achieved state-of-the-art results on various computer vision benchmarks.
