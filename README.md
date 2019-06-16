# MNIST-Handwritten-Digit-Recognition-with-Keras

## Objective
To check how the accuracy varies with the change in the number of hidden layers, epochs and other parameters and also to understand why the accuracy changed in that particular manner.

![neuralnetwork-with-one-hidden-layer](https://user-images.githubusercontent.com/51207580/59560501-99857100-9030-11e9-9806-7a020d92fa47.jpg)
### 1.How does the number of hidden layers affect the accuracy?

1 hidden layer

![hl1](https://user-images.githubusercontent.com/51207580/59560511-bf127a80-9030-11e9-92b5-49c70970800c.png)
2 hidden layers

![hl2](https://user-images.githubusercontent.com/51207580/59560515-e1a49380-9030-11e9-9d4d-9c552429587a.png)
As the number of hidden layer increases, effectiveness of backpropagation decreases; plus overfitting problem arises i.e. the network will perform very well on the training data set but the accuracy of test data set decreases.
### 2.How does the number of epoch affect the accuracy?
epoch=10
![epoch10](https://user-images.githubusercontent.com/51207580/59560690-c4bd8f80-9033-11e9-85bf-11f8b63b5069.png)
epoch=50
![epoch50](https://user-images.githubusercontent.com/51207580/59560699-d7d05f80-9033-11e9-9e80-be6d74175944.png)
As the epoch increases, the accuracy increases but the problem of overfitting may arise. So to avoid overfitting, one should set the number of epochs as high as possible and terminate training based on the error rates.
### 3.How does the number of neurons affect the accuracy?
neurons=128
![nodes128](https://user-images.githubusercontent.com/51207580/59560894-a2794100-9036-11e9-8aa7-f4dc8871c36c.png)
neurons=300
![nodes300](https://user-images.githubusercontent.com/51207580/59560898-b8870180-9036-11e9-884a-97198adbe0bd.png)
If an inadequate number of neurons are used, the network will be unable to model complex data, and the resulting fit will be poor. If too many neurons are used, the training time may become excessively long and worse the network may overfit the data. When overfitting occurs, the network will begin to model random noise in the data. The result is that the model fits the training data extremely well, but it generalizes poorly to new, unseen data. Validation must be used to test for this.
