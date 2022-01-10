# Lecture 3
### Why using a soft classifier rather than a hard classifier?
* Soft prediction returns the predicted probability of your data point belonging in one of the classes. \
  Hard label is the class your model predict given the data point.
* For example , if you are doing a two-class classification and the labels are: Fraud vs. safe. 
  If you choose soft prediction, the output of the model would look like 
 [0.9,0.1]; and the output from hard prediction would be 0 or 1
* So the soft prediction gives you more informatin about the model's confidence in prediction. 
  The higher the value for the predicted class, the more confident and accurate in the prediction will be.
  
# Lecture 4

### What is a Cost Function?
* It is a function which measures the performances of a model for given data.
* Cost function quantifier the error between predicted values and expected values and presents it in the form of a single real number.
* The goal is to reduce the cost function to zero or almost zero. 
* The ways we modify the parameters by using the Gradient Descent algorithm over the given data.


### What is Gradient Descent Algorithm?

### What is Stochastic Gradients Descent?
* Stochastic Gradient Descent minimizes the cost function using approximate gradients evaluated on mini-batches of the data.
* Using mini-batches significantly speeds up calculations
* Stochastic gradients reduce the risk of getting stuck in local minima.

### what need to be noticed when using stochastic Gradients Descent?
* Randomize data when constructing mini-batches
* Transform your inputs
* Monitor the out of sample performances
* Adaptive optimization methods do not always have good generalization

### How does SoftMax classification work?
* The softmax function is a function that turns a vector of K real values into a vector of K real values that sum to 1. 
* The input values can be positive , negetive , zero or greater than one, but the softmax transforms them into values between 0 and 1. 
* The purpose is they can be interpreted as probabilities.

### What are the learning Rates?
* The learning rate is a tuning parameter in an optimization algorithm which determinzes the step size at each iteration while
  moving toward a minimun of a loss function. 
* For sufficiently small learning rate the algorithm will converge.
* For too small will require too many computationally expensive steps
* For too large the algorithm will start oscillating or diverging.
### What are the learned weights?

### Why do you need to monitor the learning rate for GD and SGD?
* For the GD and SGD algorithm, they are sensetive for the learning rate .
* For sufficiently small learning rate the algorithm will converge.
* For too small will require too many computationally expensive steps
* For too large the algorithm will start oscillating or diverging.

# Lecture 5
### An important paper about "Learning Prpresentations by Back-Progagating Errors"

### What is a dense layer?
All inputs are densely connected to all outputs, those are called a Dense layer.


# Lecture 6
### How to use Deep learning when you have limited data?
* Try to increase diversity of data availabel for training without collecting new data
* Apply transformations to existing data such as cropping , padding , and horizontal flipping

### Why is a single layer neural network a universal function approximator?
The universal App;roximation Theorem tells us that Neural networks has a kind of unversality i.e.
no matter what f(x) is, there is a network that can approximately approach the result and do the job. 
Thsi result holds for any number of inputs and outputs.

### What is drop-out regularization?
* Dropout is a technique where randomly selected neurons are ignored druing training.
* Dropout is a regularization method that aproximates training a large number of neural networks with different architectures in parallel.
  During training, some number of layer outputs are randomly ignored or dropped out.
