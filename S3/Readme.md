## data preparation & data : 

Used dataloader from pytorch and in that injected random variable as a input in the __getitem__ along with random 
traget which is sum of random_input + label.

## combined two inputs :

Took argmax of image output and stacked with random input number and passed onto further feed forward layers.


## evaluating results : 
Made test loader using the same stratagy as the train data loder and doing evaluation on it.


## loss function : 

For image classification used cross-entropy loss as its a classification task & mse loss for random_ouput evaluation as it is regression and combined loss is propagated back to update the weights.

## Final Results:

Got greater than 97% test accuracy for 10 epochs in image classification and random number addition.

## GitHub Link : 
https://github.com/ganeshkcs/END2/blob/master/S3/MNIST-ADDITION.ipynb

