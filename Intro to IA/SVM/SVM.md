## How do they work?
###### From chatgpt
SVMs work by finding the hyperplane that maximally separates the classes in the feature space. The hyperplane is defined as a linear combination of the input features, where the weights of the linear combination are learned during the training process.

The goal of the training process is to find the hyperplane that maximally separates the classes, while also minimizing the classification error. The margin is defined as the distance between the hyperplane and the closest points of each class. SVM aims to find the hyperplane with the largest margin, which provides the best generalization performance on unseen data.

If the classes are not linearly separable, SVM uses a kernel function to map the input features into a higher-dimensional space, where the classes are more likely to be separable by a hyperplane. The most commonly used kernel functions are the linear, polynomial, and radial basis function (RBF) kernels.

Once the data has been mapped into the higher-dimensional space, SVM finds the optimal hyperplane that maximizes the margin between the classes. In the case of non-linearly separable data, SVM will find the hyperplane that best separates the classes, but may not achieve a margin that is as large as in the linearly separable case.

During prediction, SVM uses the learned hyperplane to classify new data points based on which side of the hyperplane they fall on.
## Parameters
### Gamma
Gamma (ɣ) controls how far the influence of asingle training point reaches. Lower values of gamma mean that points further away get considered when fitting the boundary. Higher values of gamma mean that points closer to the boundary carry more weight. 
What this means, effectively, is that lower values of gamma will produce a smoother result, otherwise points close to the boundary could warp it excessively.
![[SVM_gamma.svg]]

### C
C controls how much error is bearable. For larger values of C, the boundary will become more complex so as to allow for lower amount of missclassifications. 
![[SVM_C.svg]]
## Kernel

## Overfitting