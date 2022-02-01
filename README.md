# Building an Artificial Neural Network from Scratch using Python

## Prerequisites

- Python
- Basic knowledge of Supervised vs Unsupervised Machine Learning
- Familiarity with logistic regression algorithm

## Terminologies
- Neurons
- Layers
- Weights
- Vectors
- Activation functions
- Forward and Back Propagation
- Cost function
- Gradient descent

## Concept of Neural Networks – to mimic the human brain

Neurons are the basic units of our nervous system. They use electrical impulses and chemical signals to transmit information between different areas of the brain, and between the brain and the rest of the nervous system.

![Blausen_0657_MultipolarNeuron](https://user-images.githubusercontent.com/75077076/151926853-48c311d4-06cc-4d1c-ab8b-01a42eee7bf0.png)

The human brain has an average of 86 billion neurons. Neurons have three basic parts:
- a cell body: this contains the nucleus which controls the cell’s activities and contains the cell’s genetic material. 
- axon: transmits messages from the cell.
- dendrite: receives messages for the cell.

### "In machine learning, a neuron basically takes an input value, multiplies by weight (dot product), then sums all these multiplications and uses an activation function to get output."



## Training an Artificial Neural Network

The following outlines the steps involved in creating an artificial neural network from ground up

### Step 1 - Determine the architecture

There are several varieties of ANNs. The number of hidden layers, input parameters and output varies across different architectures. When creating a Neural Network, it is important to know the number of inputs there are, the number of outputs needed, and the number of hidden layers that would work best.

### Step 2 - Initialize parameters

Here, randomly initialize weights and create bias vector. 
- Weights, commonly referred to as 'w', are learnable parameters that represents the strength of the connection between units. If the weight from node 1 to node 2 has greater magnitude, it means that neuron 1 has greater influence over neuron 2.
- A bias vector is an additional set of weights in a neural network. It requires no input. Bias represents an extra neuron included with each pre-output layer and stores the value of “1,” for each action. It is commonly referred to as 'b'.

### Step 3 - Implement Forward Propagation

Forward Propagation is the process of moving from the input layer (left) to the output layer (right) in the neural network. The input data is fed in the forward direction through the network. Each hidden layer accepts the input data, processes it and passes to the successive layer until it gets to the output layer.

### Step 4 - Compute Cost Function

The cost function evaluates the performance of a neural network. It compares the predicted outputs and actual outputs and calculates the error of the model. A cost function is a single value, not a vector. It outputs a higher number if our predictions differ a lot from the actual values. This is why it is important to minimize the cost function.

### Step 5 – Implement backpropagation to compute partial derivative of the cost function

Backpropagation is the opposite of forward propagation. It is the process of moving from the output layer (right) to the input layer (left). During backpropagation (also referred to as backprop), the total loss is propagated back into the neural network to know how much of the loss every node is responsible for, and subsequently updating the weights in such a way that minimizes the loss by giving the nodes with higher error rates lower weights and vice versa.

### Step 6 – Use gradient descent or advanced optimization with backpropagation to minimize J(θ)

Gradient descent is a numerical calculation that aims to minimize the cost function. Backpropagation, as stated earlier, updates the weights so as to minimize loss.

