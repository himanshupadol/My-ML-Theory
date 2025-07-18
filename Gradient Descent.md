# The Gradient Descent

To understand the working of gradient descent, one must know the concept of derivatives, minima & maxima because the gradient means the derivative.  

In machine learning, we train a model, test it and then fine tune it for precise results. The supervised model is trained using labeled data. Labeled data means the data has records with input variables paired with output variable. The model is tested with unseen input variables in the test data to predict the output variable. These predicted output variables are compared with actual variables and the difference between them is called error.

To be a precise predictor, the model should make minimum errors.

The gradient descent algorithm is one of the various methods to minimize errors. It starts with calculating the gradient (derivative) of the error function (actual values – predicted values). The derivative represents rate of **increase** of the error with respect to weight of a feature. If the model is trained with ‘n’ input variables then the gradient vector will have ‘n’ components which define the direction of the vector.

Now the descent part. The gradient value of the error function represents direction and rate of increase of the error and hence going in opposite direction means decreasing (descent, which also means stepping down) the rate of increase of errors.

The graph of an error function is observed to be of ***convex*** shape. To find the minimum value of error for a model, we need to find the minima (minimum value) of the error function. The gradient shows the direction we should go to achieve this.

Another helping hand in gradually finding the minima is the learning rate hyperparameter (α or ή). The learning rate helps to control the rate of minimizing the error with consistent measured steps so that it does not miss the minima or a point nearest to the minima.

<img width="649" height="446" alt="gradient descent diagram" src="https://github.com/user-attachments/assets/6d538f12-a4fe-44e0-a6a1-e6c8745faa94" />
