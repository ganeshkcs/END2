## Write a neural network that can

1. take 2 inputs:
   1. an image from MNIST dataset, and
   2. a random number between 0 and 9
2. and gives two outputs:
   1. the "number" that was represented by the MNIST image, and
   2. the "sum" of this number with the random number that was generated and sent as the input to the network
      ![NN.png](https://github.com/ganeshkcs/END2/blob/master/S3/assign-2.png)   
3. you can mix fully connected layers and convolution layers
4. you can use one-hot encoding to represent the random number input as well as the "summed" output. 

## Data preparation: 

Used dataloader from pytorch and in that injected random variable as a input in the __getitem__ along with random 
traget which is sum of random_input + label.

## Combined two inputs :

Took argmax of image output and stacked with random input number and passed onto further feed forward layers.


## Evaluating results : 
Made test loader using the same stratagy as the train data loder and doing evaluation on it.


## Loss function : 

For image classification used cross-entropy loss as its a classification task & mse loss for random_ouput evaluation as it is regression and combined loss is propagated back to update the weights.

## Final Results:

Got greater than 97% test accuracy for 10 epochs in image classification and random number addition.

## GitHub Link : 
https://github.com/ganeshkcs/END2/blob/master/S3/MNIST-ADDITION.ipynb

