## Defining an L-layer Neural Network to classify cat images<br />
The order of functions to make a nueral network model for classification:

1) Begin by importing required packages (GOTO [a link](https://github.com/Farzane-Ka/deep-learning/blob/main/nn-image-classification/packages) )
1) Train with the function: L_layer_model(X, Y, layers_dims, learning_rate = 0.0075, num_iterations = 3000, print_cost=False)
   * This function first initializes the parameters W (weights) and b (bias) to random values.
  
   * For num_iterations, loops through and computes the gradient decent for the cost function:
    * makes a forward propagation, computes the cost, makes a backward propagation:
  
    * AL, caches = L_model_forward(X, parameters)
    * cost=compute_cost(AL, Y)
    * grads= L_model_backward(AL, Y, caches)
    * parameters=update_parameters(parameters, grads, learning_rate)
  
2) To make a model for training:
    - parameters, costs = L_layer_model(train_x, train_y, layers_dims, num_iterations = 3000, print_cost = False)
    
3) To compute the accuracy:
    - pred_train = predict(train_x, train_y, parameters)
  
