# Previous concepts
These concepts are relevant to get some information for the concepts that we're going to work later. I divided because they are implicit in later concepts so understanding these are helpful for the next ones. 

## More generic lexicon tha is applied here

### Query
[Define a query in general and if there is a difference between query and prompt]

### Pipeline 
Pipeline is a set of data-processing stages, where the output of the previous task is used as input for the next one. This allows for big tasks to be broken down into smaller ones and for the tasks themselves to run concurrently or sequentially.

In neural networks, a pipeline is a multi-stage process where tasks like data preprocessing, feature extraction, model training, tuning, evaluation, and deployment are performed in sequence

### Architecture of a system
[Define what is the architecture of a system with several examples, one of them related to Artificial inteligence]

### Decision algorithm 
[Define what is a decision algorithm with several examples, one of them related to Artificial inteligence]

### Deployment of a system 
[Define a bit what is the deployment of a system with a several examples, one of them related to Artificial Inteligence]

## Deep learning
[Define what is deep learning and its limitations]


## Neural network
[Define Neural Network with examples and explaining the concepts bellow]

### Hyperparameter (in a neural network)

### Layer of a neural network

### Input layer

### Hidden layer

### Output layer

## Gradient of a function (and relationship with Neural Networks)
A gradient is a vector showing the direction of the greatest increase of a function. The module of the gradient vector shows the rate of change of the function. For example, Let's look at the graph of the parabola y=x². 
The figure shows point A with coordinates (2, 4) and visualized the gradient in it. It is clear that the resulting arrow points in the direction of growth. The sign before y is called nabla, this is the generally accepted notation for the gradient. This entry says: here is the gradient of the function y(x) drawn. 

Neural network. 
A neural network is a tool for restoring the relationship between input data and output. Each neuron multiplies the data from each of its inputs by a connection weight that determines how important this data is, and then sums up (this sum is called weighted) all the data. After this, the neuron is "activated" - it passes the data on if the sum found is greater than a certain value. Otherwise, it fades out, and the data does not go to other neurons.  
Example of the simplest fully connected neural network, each layer of which consists of one neuron. Here, the connection weights are w1, w2, w3, and w4, Σ is the adder, and φ is the activation function: 
X-> W1 -> ∑; ϕ  -> W2 -> ∑; ϕ  -> W3 -> ∑; ϕ  -> W4 -> Y 
A person prepares data for the neural network in the format (input-data, expected-response). Then the following happens: 
1. The neural network runs the input data through itself, receives an answer (most likely incorrect); 
2. The neural network compares the received answer with the correct one, finds an error (for example, by subtracting its answer from the given one); 
3. Based on the calculated error, the neural network determines how to change the connection weights so that the error becomes smaller; 
4. The neural network changes the weights, reducing the error; 
This cycle is repeated many, many times on different data so that the neural network understands well what is required of it. But then, if we give the neural network data that it has never seen, it will give us the correct answer, because it itself has determined the relationship between the input data and the result and has learned to reproduce it. 

The relationship between the gradient and the neural network. 
The neural network must find the error between its output and the correct answer each time, and then determine how to change the weights to reduce the error. It turns out that there is a very, very complex dependence of the error on all the parameters of the neural network. That is, 
L = f(w1, w2, w3, …, wn), 
where L is the error, and f(w1, w2, w3, …, wn) is a function of the weights of the connections in the neural network. I think it is worth clarifying here why the error depends on the parameters of the model (this is how we will sometimes call neural networks): the neural network cannot influence the answer prepared by a person, but it can change its answer (which depends on all the parameters of the model) so that the error becomes smaller. 
That is, the main task of the neural network during training is to find the minimum of the error function - that is, to calculate such values of the weights of the connections that with them the error will be minimal (that is, the answer of the neural network will be as close as possible to the answer prepared by a person). 
If the gradient pointing in the direction of the function's fastest growth is simply turned 180 degrees, it will point in the opposite direction: the direction of the function's fastest decay. This property will help us gradually "descend" to the minimum of the error function. 

## Dataset
[Define what is a dataset of a Deep learning network with some examples. Try to get specific]


## Large language model (LLM)
[Define and expand a bit, are there other types of models that are not large or not about language?]


## Natural language processing model 
[Define what is it and the difference between this concept, an LLM and the concept of Natural Language Understanding]

## Machine-actionable information
[Define what is machine-actionable information and what is not or how do create it]

## Extra ball: Tensor
[Define what is a tensor with your words so your colleagues can more less understand it]

[some information here](https://en.wikipedia.org/wiki/Tensor_(machine_learning))


---
