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
  
# Lecture 7
### What is bias-variance tradeoff?

### If we cannot understand why an AI made a decision, how will we know when the decision is wrong or right?
* Layer-wise Prlevance Propafation(LRP)

# Lecuture 8
### What is pooling?
* The pooling layer is commonly applied after a convolution layer to reduce the spatial size of the input. It is applied independently to each depth slice of the input valume,
* Perform a sub-sampling at every depth
* Replace a region by a single neuron
* There are two different types of pooling, Maxinum Pooling and Average Pooling.
### How does the filter convolution work?
* We have a input , such as an image of pixel values, and we have a filter, which is a set of weights,
  and the filter is systematically applied to the input data to create a feature map.
### Waht is Correlation
A correlation si a measure of the direction and the size of two or more variables in a data set.
This means that when looking at statistical models, if one variable changes or moves in a specific direction,
Then another variable does too. When behaviors like thsi appear between variables in studies, satitsticians assume a correlation,
or link, between the samples. 
* The primary types of correlations can occur in any given study:
* Positive correlations represent a positive change in one variable because of another
* Negative correlations represents a negative change in one variable becasue of another
* A zero correlative relationship indicates there is no apparent link between two or more vaiables.
### What are spruious correlations in high-d?
Spurious correlation in statictics represents a connection between two variables that seems to be a causal relationship but really is not.

# Lecture 9
### What is High Dimensional Data?
* High Dimensional data refers to a dataset in which the number of features p is larger than the number of observations N, often written as p>>N.
* When the number of features in a dataset exceeds the number of observations, we will never have a deterministic answer.
* It becomes impossible to find a model that can describe the relationship between the predictor variables and the response variable because we do not have 
  enough observations to train the model on.
  
  
* 
### What is the effective dimensionality of a data set?
### What is a PCA?
* Principal Component Analysis or PCA is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets,
  by transforming a large set of variables into a smaller one that still contains most of the information in the large set.
* The idea of PCA is simple, reduce the number of variables of a data set, while preserving as much information as possible.
### What is the step of PCA
* Standardization
  The aim of this step is to standardize the range of the continuous initial variables so that each one of them contributes equally to the analysis.
* Covariance Matrix Computation
  The aim of this step is to understand how the variables of the input data set are varying from the mean with respect to each other, or to see if there 
  is any relationship between them.
* Compute the eigenvectors and eigenvalues of the covariance matrix to identify the principal components.

# Lecture 10
### What is the DBSCAN method?
DBSCAN estimats a density in a Neighborhood around every data point.
* The algorithm does not require to specify the number of clusters
* The algorithm has an computational cost of O(NlogN)
* It works well with noisy data
* It is great at separating clusters of high density versus clusters of low density within a given dataset
* It is great with Handling ourliers within the datset
### How does the K-means algorithm work?
* K-means is the most famous topics under the realm of Unsupervised Learning in machine learning.
* K-means takes data points as input and groups them into k clusters.
* K-means is just a clustering algorithm. It uses the distance between points as a measure of similarity, based on k averages(means)
* The idea behind k_means is that, we want to add k new points to the data we have. Each one of those points called a Centroid will be going around trying 
  to center itself in the middle of one of the k clusters we have. Once those points stop moving , our clustering algorithm stops.
  
### Waht is a data anomaly?
* A data that falls outside of what is acceptable is a data anomaly.

