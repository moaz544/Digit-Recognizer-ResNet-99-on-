
Prediction Competition:
https://www.kaggle.com/c/digit-recognizer




# Digit-Recognizer-ResNet-99-on-
In this post, we will try the ResNet for image recognition. We will learn the Keras application tutorial for ResNet engineering from scratch. (Residual networks) is a deep neural network that is used as a backbone for many computer vision applications such as object detection, image segmentation, etc.

Distinguished by the ResNet syntax, a "shortcut" or "skip connection" allows for the gradient to be re-propagated directly to previous layers

![ResNet-Residual-Network-Architecture-Skip-Connections](https://user-images.githubusercontent.com/73136710/108855013-2c8df100-75f1-11eb-8239-be1adabad784.png)



# Identity Block

Identity block is the standard block used corresponding to the case where the input activation has the same dimensions as the output activation.

![ResNet-Residual-Network-Keras-Implementation-Identity-Block](https://user-images.githubusercontent.com/73136710/108855018-2dbf1e00-75f1-11eb-99db-f0869a963ee8.png)


# Convolutional Block
We can use this type of block when the input and output dimensions don’t match up. The difference with the identity block is that there is a CONV2D layer in the shortcut path.

<img width="647" alt="0mE2p" src="https://user-images.githubusercontent.com/73136710/108855019-2dbf1e00-75f1-11eb-9522-784179179c49.png">

