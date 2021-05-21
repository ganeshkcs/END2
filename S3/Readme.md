## Write a neural network that can

1. Take 2 inputs:
   1. An image from MNIST dataset, and
   2. A random number between 0 and 9
2. And gives two outputs:
   1. The "number" that was represented by the MNIST image, and
   2. The "sum" of this number with the random number that was generated and sent as the input to the network
      ![NN.png](https://github.com/ganeshkcs/END2/blob/master/S3/assign-2.png)   
3. You can mix fully connected layers and convolution layers
4. You can use one-hot encoding to represent the random number input as well as the "summed" output. 

## Data preparation: 

Created custom dataset which downloads MNIST dataset and implemented  __getitem__ function which returns image, label random_ input, random 
traget which is sum of random_input + label.

## Combined two inputs :

Took argmax of image output and stacked with random input number and passed onto further feed forward layers.


## Evaluating results : 
Evaluated test the results by splitting the dataset into in train set and test set and also caluating the accuracy for image and additon of random number.


## Loss function : 

For image classification used cross-entropy loss as its a classification task & mse loss for random_ouput evaluation as it is regression and combined loss is propagated back to update the weights.

## Final Results:

Got greater than 97% test accuracy for 10 epochs in image classification and random number addition.

## GitHub Link : 
https://github.com/ganeshkcs/END2/blob/master/S3/MNIST-ADDITION.ipynb

