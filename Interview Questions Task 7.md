1. What is a support vector?
Support vectors are the data points that are closest to the decision boundary (or hyperplane) in an SVM model. These points are crucial because they directly influence the position and orientation of the hyperplane. Removing or changing a support vector would significantly alter the decision boundary, making them the backbone of the SVM model.

2. What does the C parameter do?
The C parameter in SVM controls the trade-off between maximizing the margin and minimizing classification error.
A large C value gives more importance to correctly classifying training points, potentially leading to overfitting.
A small C value allows more misclassifications but generally results in a wider margin, making the model more robust to noise.
Think of C as a way to control how much you punish the model for making mistakes.

3. What are kernels in SVM?
Kernels are functions that transform data into a higher-dimensional space, making it easier to separate with a linear boundary. They allow SVM to work efficiently in complex scenarios where data isn't linearly separable.
Linear Kernel: Directly finds a linear decision boundary.
Polynomial Kernel: Projects data into higher polynomial dimensions.
RBF (Radial Basis Function) Kernel: Maps data to an infinite-dimensional space, making it good for capturing complex patterns.
Choosing the right kernel depends on the dataset's characteristics and complexity.

4. What is the difference between linear and RBF kernel?
Linear Kernel: Works well when data is linearly separable or almost linear. It draws a straight line (or hyperplane) as the decision boundary.
RBF Kernel: Suitable for more complex and non-linear data. It maps the data into a higher-dimensional space and finds a curved decision boundary.
If your data has complex relationships that a straight line can't capture, RBF is usually the better choice.

5. What are the advantages of SVM?
Effective in high-dimensional spaces: Works well even when the number of features exceeds the number of samples.
Memory-efficient: Uses support vectors rather than all data points.
Versatile: By choosing appropriate kernels, it can perform well with both linear and non-linear data.
Robust to overfitting (especially with high-dimensional data): Controlled by the C parameter and the use of margin maximization.

6. Can SVMs be used for regression?
Yes! SVM can be used for regression tasks using SVR (Support Vector Regression). Instead of finding a decision boundary, it tries to fit a function that deviates from the actual outputs by at most a specified margin while keeping the model as flat as possible.

7. What happens when data is not linearly separable?
If the data isn't linearly separable, SVM can still work by:
Soft Margin: Allowing some points to be on the wrong side of the margin, controlled by the C parameter.
Kernel Trick: Transforming data into a higher-dimensional space where it becomes linearly separable.
This makes SVM powerful for dealing with real-world, messy data.

8. How is overfitting handled in SVM?
Overfitting is primarily controlled by
Regularization (C parameter): Reducing C increases the margin at the cost of allowing more classification errors, leading to a simpler, more generalized model.
Kernel Choice: Complex kernels like RBF can overfit if hyperparameters (like gamma) are not properly tuned.
Cross-Validation: Helps ensure that the model performs well on unseen data rather than just the training data.