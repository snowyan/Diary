#Machine Learning
* Any learning preblem can be cast into an optimization problem by minimizing a risk function
* The best function h in the space of all hypotheses H for the prediction task is the one associated the lowest empirical risk.
# Lecture 1
### How would you define Machine Learning?
* Machine Learning is a method of data analysis which automates analglical model building. It is a bunch of artificial intelligence based on the idea that 
  system can learn from data , identify pattern and make dicisions with minimal human intervention.
### What are the two most common supervised learning task?
Classification and regression 
# Lecture 2
### Can you derive the Bayes optimal predictor for a square loss function?

### Why is a good fit to the data not necessarily a good predictor
### About the Bias-Variance tradeoff
* To choose a hypothesis class we need to consider the Bias-Variance-tradeoff
* more complex models reduce bias at some point the model complexity is too high to be fitted by the data and the variance increases.
# Lecture 3
### Hard classification
* Perceptron ( hard classification)
* it is not differentiable
* it is not useful in case of noisy data when a unique classificatin is not possible
### Soft classifier
* Logistic or sigmoid function
* retrurn the probability fo being in category n
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
* GD algorithm searchs optimal w by going downhill
* GD only finds local minima of the risk or cost function
* GD are computationally expensive to computer for large datasets
* GD is sensitive to the choice of learning rate
* GD treats all directions of the parameter space uniformly
* GD is sensitive to initial conditions
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
### Common activation functions
* For sigmoids and hyperbolic tangent functions the gradient vanishes when input weights become large
* Vahishing gradients are a feature of saturation
* The gradients of ReLUs and ELUs is finite also for large inputs
### Why do we need non-linear activation functions?
* Linear activation functions can only fit linear decision boundaries
* Non-linear activation functions can fit complex decision boundaries
* Activation function need to be non-linear
### Neural Network
* NNs are hierarchical layers of neurons
* NNs can approximate any function but we need sufficiently large data to fit all w.
* The four categories: 
   1 general purpose neural networks for supervised learning
   2 DDNs designed for image processing ex:CNNs
   3 Neural Networks for sequential data ex: Recurrent Neural Networks(RNNs)
   4 Neural Networks for unsupervised learning ex: Deep Boltzmann Machines

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

# Question
### What is Bias?
* Bias is the simplifying assumptions made by the model to make the target function easier to approximate.
### What is Variance?
* Variance is the amount that the estimate of the target function will change given different training data
### What is Trade-off?
* Trade-off is tension between the error introduced by the bias and the variance.
### What do you expect will happen with bias and variance as you increase the model of complexity?
* Following the increase the model of complexity the bias is decrease and variance is increase.
### What do you expect will happen with bias and variance as you increase the size of training data for a given model?
* Bias decrease and vaiance is increase.
### Do some online quiz
### When using the Back-Propagation learning algorithm, what exactly is back-propagated , and from where to where?
* Backpropagation algorithm is the most fundamental building block in a neural network. The algorithm is used to effectively train
a neural network through a method called chain rule. After each forword pass through a network, backpropagation performs a backword pass while adjusting the moels parameters(weights and biases)
### The basic equation for gradient descent training is this. Describe what the symbols in it refer to and how it can be used to derive a training algorithm for a multi-layer perceptron.(MLP)
### Explain the main reason why a back-propagation training algorithm might not find a set of weights which minimizes the training error for a given feed-forward neural network.
The back propagation stragegy is a steepest gradient method, a local optimization technique, Therefore it can become locked in a local optimum.
### State one advantage of linear rectified activation compared to logistic sigmoid activation
Compared to logistic sigmoid activation the advantage of linear rectified activation is the reduced likelihood of the gradient to vanish.
Orther is ReLUs are sparsity and faster. More computationally efficient to compute.
### Does it make sense to initialize all weights in a deep network to 0?
* Zero initialization causes the neuron to memorize the same funcitons almost in each iterations and product the same outputs.
* Random initialization is a better choice but initializing much high or low value can result in slower optimization
* Use He initialization can solve the above issue to some extent.
### Which eigenvalue indicates the direction of the largest varicance in the dataset?
The eigenvector with the largest eigenvalue is the direction along with the data set has the maximum variance.
### Draw and explain an example where t-SNE work better than PCA

### What is t-SNE?
t-SNE is t distributed stochastic neighbourhood embedding.
### What is K-Mean?
K-Mean is a simple clustering algorithm. 
### How to caculate the K-Mean?
* Step1: Selelct the centroids
* Step2: Caculate the distance between every point and centroids.
* Step3: Compare the vaue of the step2, the smaller one is belong to conrespond cluster.
* Step4: Follow the step3's cluster result and average the same culster's value and modify the centriods values
* Step5: Go back to Step2 until the cluster classificatin is the same.
### What is egglomerotive cluster?
* egglomerotive use a bottom-up approch
* each data points starts in its own cluster
* by taking the two most similar clusters tegother and merge them
### What is Divisive cluster?
* divisive use a top-down approch
* all data points start in the same cluster
