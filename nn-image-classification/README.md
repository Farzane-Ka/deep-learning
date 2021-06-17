The order of functions to make a nueral network model for classification:

1)Train with the function:

  1) L_layer_model(X, Y, layers_dims, learning_rate = 0.0075, num_iterations = 3000, print_cost=False)
  2) This function first initializes the parameters W (weights) and b (bias) to random values.
  
  3) For num_iterations, we loop through and compute the gradient decent for the cost function:
  4) make a forward propagation, compute the cost, make a backward propagation:
  
  5) AL, caches = L_model_forward(X, parameters)
  6) cost=compute_cost(AL, Y)
  7) grads= L_model_backward(AL, Y, caches)
  8) parameters=update_parameters(parameters, grads, learning_rate)
  
2) To make a model for training:
    1) parameters, costs = L_layer_model(train_x, train_y, layers_dims, num_iterations = 3000, print_cost = False)
    
3) to compute the accuracy:
    1) pred_train = predict(train_x, train_y, parameters)
  
