Training an SVM manually involves implementing the optimization problem that SVM solves, which is a convex optimization problem with a quadratic objective function and linear constraints. There are many optimization algorithms that can be used to solve this problem, such as gradient descent, stochastic gradient descent, and quadratic programming.

Implementing an SVM manually can be quite challenging, and requires a good understanding of optimization theory and algorithms. However, if you're interested in learning how to do this, here's a high-level overview of the steps involved:

1.  Define the optimization problem: The SVM optimization problem involves minimizing a convex quadratic function subject to linear constraints. The objective function is typically formulated to maximize the margin between the classes, subject to a constraint that the data points are correctly classified.
    
2.  Choose a solver: There are many optimization algorithms that can be used to solve the SVM optimization problem. Some popular ones include gradient descent, stochastic gradient descent, and quadratic programming. The choice of solver depends on the size of the dataset and the complexity of the problem.
    
3.  Implement the solver: Once you have chosen a solver, you need to implement it in code. This involves defining the objective function and the constraints, and then running the optimization algorithm to find the optimal solution.
    
4.  Evaluate the solution: Once you have obtained the optimal solution, you need to evaluate it to see how well it performs on the training data. This involves calculating the accuracy, precision, recall, and F1 score of the classifier.
    

Overall, training an SVM manually can be a challenging task, and is not recommended unless you have a good understanding of optimization theory and algorithms. In practice, it's much easier to use a pre-built SVM implementation, such as the one provided in the Scikit-learn library.