# Analysis-of-Boston-Housing-Dataset-Perceptron-Algorithm-and-Neural-Networks

This project involves implementation of the Rosenblatt's algorithm, commonly known as the perceptron algorithm, and utilizing out-of-the-box neural networks for regression analysis. Here is a breakdown of the tasks performed:

- Imported necessary libraries such as matplotlib.pyplot, pandas, sklearn.datasets, and sklearn.model_selection.
- Loaded the Boston housing dataset using the load_boston() function from sklearn.datasets.
- Created a pandas DataFrame named boston_df from the dataset, including the target variable 'MEDV' and a binary column 'high-Priced' indicating whether a house is considered high-priced or not.
- Visualized the dataset by creating a scatter plot of the 'RM' (average number of rooms per dwelling) against 'MEDV' (median value of owner-occupied homes). High-priced and low-priced homes were differentiated using distinct colors.
- Prepared the data for training by separating the feature variables into X and the target variable into Y.
- Added a column of ones to the feature matrix X to account for the bias term in the perceptron algorithm, using np.c_.
- Initialized the step size, weights, and error variables required for the perceptron algorithm.
- Defined the myPerceptron function, responsible for performing a single iteration of the perceptron algorithm. This function updated the weights based on the prediction and target values.
- Applied the myPerceptron function iteratively until convergence, counting the number of errors in each iteration and storing them in the error_list.
- Plotted a graph showcasing the number of errors versus the iteration number to visualize the convergence of the perceptron algorithm.
- Printed the number of iterations required for convergence and provided additional analysis regarding the convergence rate and the relevance of gradient descent.
- Visualized the separation line obtained from the perceptron algorithm by overlaying it on the scatter plot, thereby demonstrating the classification boundary between high-priced and low-priced homes.
- Split the data into training and testing sets using the train_test_split function from sklearn.model_selection.
- Constructed single-hidden-layer neural networks with various sizes, trained them on the training set, and evaluated their performance based on R-squared scores and mean squared errors on both the training and test sets.
- Repeated the above step for two-hidden-layer neural networks with different sizes, reporting their performance metrics.
- Further repeated the process by varying the number of neurons and hidden layers in the neural networks, assessing their performance on the training and test sets.
- Utilized SHAP (SHapley Additive exPlanations) to explain the predictions made by the best-performing neural network model.
- Generated a summary plot illustrating the impact of different features on the predicted house prices.
- Created waterfall plots to elucidate the predictions for multiple instances using SHAP values.
- Conducted an analysis concerning the discriminatory features employed by the model and highlighted ethical concerns related to potential bias in the model's predictions.
