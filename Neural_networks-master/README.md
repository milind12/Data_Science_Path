# Neural_networks

## Dataset

iris.csv dataset has the following features:

1. sepal_length - Continuous variable measured in centimeters.
  
2. sepal_width - Continuous variable measured in centimeters.
	
3. petal_length - Continuous variable measured in centimeters.
	
4. petal_width - Continuous variable measured in centimeters.
	
5. species - Categorical. 2 species of iris flowers, Iris-virginica or Iris-versicolor.

## Sigmoid_activation function

sigmoid_activation has inputs x, a feature vector, and, theta, a parameter vector, of the same length to implement the sigmoid activation function. 

## Singlecost function

It computes the cost from just a single observation.

1. It uses input features X, targets y, and parameters theta to compute the cost function.

2. Then it is called to assign the cost of variables x0, y0, and theta_init to variable first_cost.


## Multiplecost function

multiplecost() estimates the cost of two layer neural network.

1. It uses the observations in X, targets y and inital parameters theta0_init and theta1_init.

2. It assign the cost to variable c.

## Model

NNet3 class in scikit-learn takes 4 parameters for instantiation learning rate(used in gradient descent), maxepochs (max iterations for gradient descent), convergence_thres (costs convergence threshold i.e prev-curr > convergence_thres) and hidden units.

### Train, predict and test

Train the neural network using features, target and model, which has been initialized with a set of parameters. 

Once training is complete, use the predict() function to return the probabilities of the flower matching the species Iris-versicolor.

Compute the AUC score, using roc_auc_score() and assign it to auc




