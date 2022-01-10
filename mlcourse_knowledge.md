### Why using a soft classifier rather than a hard classifier?
* Soft prediction returns the predicted probability of your data point belonging in one of the classes. \
  Hard label is the class your model predict given the data point.
* For example , if you are doing a two-class classification and the labels are: Fraud vs. safe. 
  If you choose soft prediction, the output of the model would look like 
 [0.9,0.1]; and the output from hard prediction would be 0 or 1
* So the soft prediction gives you more informatin about the model's confidence in prediction. 
  The higher the value for the predicted class, the more confident and accurate in the prediction will be.

### What is a Cost Function?
* It is a function which measures the performances of a model for given data.
* Cost function quantifier the error between predicted values and expected values and presents it in the form of a single real number.
* The goal is to reduce the cost function to zero or almost zero. 
* The ways we modify the parameters by using the Gradient Descent algorithm over the given data.


### What is Gradient Descent Algorithm?
