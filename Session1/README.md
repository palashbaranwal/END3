**TSAI - ENDv3 - Session 1**

**Session 1 - Background & Very Basics**

1. Rewrite the Colab file and:
   1. Remove the last activation function
   2. Make sure there are in total 44 parameters
   3. Run it for 2001 epochs

2. You must upload your assignment to a public GitHub Repository and share the link as the submission to this assignment

3. Add a readme file to your project and describe these things:
   1. What is a neural network neuron?
   2. What is the use of the learning rate?
   3. How are weights initialized?
   4. What is "loss" in a neural network?
   5. What is the "chain rule" in gradient flow?


**Questions**



1. What is a neural network neuron?

    - A Neural Network neuron is similar to a biological neuron where a set of neurons organized in layers.
    - It receives input from the other neurons, performs some processing, and produces an output.
    - The inputs can be the feature values of a sample of external data, such as images or documents, or they can be the outputs of other neurons.
    - Each neuron is a mathematical operation that takes it's input, multiplies it by it's weights and then passes the sum through the activation function to the other neurons.
    - The outputs of the final output neurons of the neural net accomplish the task, such as recognizing an object in an image.

2. What is the use of the learning rate?

    - The amount that the weights are updated during training is referred to as learning rate, often in the range between 0.0 and 1.0.
    - The learning rate hyperparameter controls the rate or speed at which the model learns.
    - Specifically, it controls the amount of apportioned error that the weights of the model are updated with each time they are updated, such as at the end of each batch of training examples.
    - Given a perfectly configured learning rate, the model will learn to best approximate the function given available resources.

3. How are weights initialized?

    - Main objective of weights initialization is to prevent layer activation outputs from exploding or vanishing gradients during the forward propagation.
    - If either of the problems occurs, loss gradients will either be too large or too small, and the network will take more time to converge if it is even able to do so at all.
    - If we initialized the weights correctly, then our objective i.e, optimization of loss function will be achieved in the least time.
    - Tanh saturates at large positive or large negative values, the gradient still vanishes at saturation.

HOW?:

    - The mean of the activations should be zero.
    - The variance of the activations should stay the same across every layer.
    - All the weights of layer are picked randomly from a normal distribution with mean=0 and standard deviation=1
    - Although over the last decade, more specific heuristics have been developed that use information, such as the type of activation function that is being used and the number of inputs to the node.

4. What is "loss" in a neural network?

   - Prediction error of Neural Net. Difference between predicted and actual value.
   - Loss is used to calculate the gradients.
   - And gradients are used to update the weights of the Neural Net.
   - With neural networks, we seek to minimize the error.
   - The objective function is often referred to as a cost function or a loss function and the value calculated by the loss function is referred to as simply “loss.”

5. What is the "chain rule" in gradient flow?

   - The chain rule is used for calculating the derivative of composite functions.
   - In neural networks this rule is used to carry out Backpropogation and compute the effect of the node on the gradients flowing back from right to left in neural network.
   - If a variable z depends on the variable y, which itself depends on the variable x, so that y and z are dependent variables, then z, via the intermediate variable of y, depends on x as well.
   - Mathematically written as: 1_7PhAl-QqLAc5vIOjEAQ-BA
   - Here X = Input bih=bias w= weights E= error (calculated using mean squared error here) 
