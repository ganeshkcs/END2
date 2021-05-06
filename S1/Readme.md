# Assignment:

## What is a neural network neuron?

Neural network neurons are similar to the biological neurons where they take an input, act on the input with an activation fuction and gives us an output. A                single neuron will look as shown below.

![Neuron](https://github.com/ganeshkcs/END2/blob/master/S1/Neuron.png)

Collection of such neurons will form a neural network.

![Neural-Network](https://github.com/ganeshkcs/END2/blob/master/S1/Neural-network.png)

## What is the use of learning rate?

We know that at the end of forward propagation in neural network there would be difference between the actual value and the predicted value, this difference is between actual and predicted value is called as Loss/Error/Cost. To reduce the loss we need to update the weights and biases and this process is achieved by back propagation where based on the loss, the weights and biases that comes as input ( from previous hidden layer ) to the output is updated, similarly all the other layers  ( except the layer 1 or the input layer ) are also updated. 
                   
 If we plot a graph between the weight and cost ( Y axis ) as shown below 
 
 ![LR](https://github.com/ganeshkcs/END2/blob/master/S1/lr_different_ones.png)

 To achieve the minimum point in the graph we should know two things
 
 1. In which direction we should move
 2. How much we should move ( Learning Rate )

 So we should always update the weights such that it moves towards the minimum loss, which is given by the below equation.
 
 new_weight = existing_weight — learning_rate * gradient
 
Learning rate is a hyper-parameter that controls how much we are adjusting the weights of our network with respect the loss gradient. The lower the value, the   slower we travel along the downward slope.
 
Typically learning rates are configured naively at random by the user. At best, the user would leverage on past experiences (or other types of learning material) to gain the intuition on what is the best value to use in setting learning rates.
 
 




