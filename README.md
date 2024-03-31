Supervised –  we use the labeled/classified data to train the machines.

Unsupervised – we do not have labeled/classified data to train the machines.

Reinforced –  we train the machines through rewards on the right decisions.

# Super Vector Machine  (SVM): (e.g., high dimensional data--text or image classification)
Support Vector Machine (SVM) is a supervised machine learning algorithm used for both classification and regression.

SVM is a versatile algorithm that can be used for classification and regression tasks, particularly when dealing with small to medium-sized datasets, high-dimensional spaces, 
and when a clear margin of separation exists between classes.

A support vector machine (SVM) is a supervised learning algorithm used for classification tasks. It works by finding the hyperplane that best separates the classes in the feature space while maximizing the margin between the classes. 

# When to Use SVM (Classification: multiclass family):
1) Binary or Multiclass Classification:
2) Clear Margin of Separation: SVM works well when there is a clear margin of separation between classes. If the classes are linearly separable or nearly separable, SVM can be a good choice.
3) High-Dimensional Data: When dealing with high-dimensional data, such as text or image classification, SVM can perform well. It is effective in such scenarios because it constructs a hyperplane
   to separate the classes in the feature space.
4) Robustness to Overfitting:SVM aims to maximize the margin between classes, which helps in generalizing well to unseen data and prevents overfitting, making it suitable for datasets with noisy or complex patterns.

# Note: 
If the data points are plotted in a 2-dimensional graph, then the decision boundary (similar to the line of best fit) is referred to as a straight line. However, if there are more than two dimensions, these are referred to as hyperplanes. While there may be multiple hyperplanes that separate the classes, SVM chooses the one with the maximum distance between the classes to distinguish classes clearly.

SVM is different from the classification due to the Kernel. So, kernels are a class of algorithms used for pattern analysis in the SVM.

SVMs without kernels may have similar performance as that of logistics regression algorithm. Unlike the logistic regression algorithm which considers all data points, the support vector (data poiints) classifier only considers the data points closest to the hyperplane i.e. the Support Vector

# When to Use SVR (Regression--non-linaer relationship):

1) Continuous Target Variable: SVR is suitable for regression tasks where the target variable is continuous rather than categorical. It can predict numerical values based on input features.

2) Non-linear Relationships: SVR is capable of capturing non-linear relationships between features and the target variable through the use of kernel functions.
   It can handle complex data patterns and non-linear relationships effectively.

3) Robustness to Outliers: SVR is less sensitive to outliers compared to some other regression techniques, as it focuses on minimizing errors within a specified margin (epsilon-insensitive loss function).
   This makes it suitable for datasets with outliers or noisy data.

4) Small to Medium-Sized Datasets: SVR can work well with small to medium-sized datasets, especially when the relationships between features and the target variable are complex and non-linear.

# Considerations: SUPER VECTOR REGRESSION vs REGRESSION and SUPER VECTOR  CLASSIFICATION vs CLASSIFICATION

A) Data Size: SVM and SVR can both handle small to medium-sized datasets efficiently. However, for very large datasets, training SVM/SVR models can be computationally expensive.

B) Data Complexity: SVM is typically used for classification tasks with clear margin separation, while SVR is used for regression tasks with non-linear relationships.

C) Interpretability: SVM provides interpretable results in classification tasks (e.g., decision boundaries), while SVR may not provide as straightforward interpretation in regression tasks.



# Support Vector Machine Terminology

Hyperplane: Hyperplane is the decision boundary that is used to separate the data points of different classes in a feature space.
In the case of linear classifications, it will be a linear equation i.e. wx+b = 0.

Support Vectors: Support vectors are the closest data points to the hyperplane, which makes a critical role in deciding the hyperplane and margin. 

Margin: Margin is the distance between the support vector and hyperplane. The main objective of the support vector machine algorithm is to maximize the margin. 
The wider margin indicates better classification performance.

Kernel: Kernel is the mathematical function, which is used in SVM to map the original input data points into high-dimensional feature spaces, so, that the hyperplane can be easily found out
even if the data points are not linearly separable in the original input space. Some of the common kernel functions are linear, polynomial, radial basis function(RBF), and sigmoid.

Hard Margin: The maximum-margin hyperplane or the hard margin hyperplane is a hyperplane that properly separates the data points of different categories without any misclassifications.

Soft Margin: When the data is not perfectly separable or contains outliers, SVM permits a soft margin technique.
Each data point has a slack variable introduced by the soft-margin SVM formulation, which softens the strict margin requirement and permits certain misclassifications or violations. 
It discovers a compromise between increasing the margin and reducing violations.

Parameters: SVM has hyperparameters like C (regularization parameter), epsilon (the size of the epsilon-insensitive tube), and the choice of kernel (linear, polynomial, radial basis function, etc.). 
Margin maximisation and misclassification fines are balanced by the regularisation parameter C in SVM. The penalty for going over the margin or misclassifying data items is decided by it.
A stricter penalty is imposed with a greater value of C, which results in a smaller margin and perhaps fewer misclassifications.

Hinge Loss: A typical loss function in SVMs is hinge loss. It punishes incorrect classifications or margin violations. 
The objective function in SVM is frequently formed by combining it with the regularisation term.

Dual Problem: A dual Problem of the optimisation  requires locating the Lagrange multipliers related to the support vectors can be used to solve SVM. 
The dual formulation enables the use of kernel tricks and more effective computing.





![image](https://github.com/Tiwari666/Super-Vector-Machine-SVM-/assets/153152895/289315d7-add6-4187-8bc6-904cb441b0fa)


![image](https://github.com/Tiwari666/Super-Vector-Machine-SVM-/assets/153152895/a36d6a5d-cb69-4cbb-9c87-f71e32162026)


![image](https://github.com/Tiwari666/Super-Vector-Machine-SVM-/assets/153152895/1980f8e7-3796-473f-bb5c-7c154c5557da)

![image](https://github.com/Tiwari666/Super-Vector-Machine-SVM-/assets/153152895/a70ba277-270c-40c7-93fc-cfede7d66a60)

# How SVM works?
A) Finding the Hyperplane: SVM aims to find the hyperplane that best separates the two classes. This hyperplane is the decision boundary.

B) Maximizing Margin: SVM not only finds a separating hyperplane but also aims to maximize the margin, which is the distance between the hyperplane and the nearest data points (support vectors) from each class. This margin maximization is crucial because it helps SVM generalize better to unseen data.

C) Dealing with Non-Linear Data: In cases where the data is not linearly separable, SVM uses a technique called the kernel trick. It maps the input data into a higher-dimensional space where it might become linearly separable. Common kernel functions include linear, polynomial, radial basis function (RBF), and sigmoid.

D) Classification: Once the hyperplane is determined, classifying new data points involves checking which side of the hyperplane they fall on. If a point lies on one side, it belongs to one class; if it lies on the other side, it belongs to the other class.


SOURCES:
1. Link1: https://www.geeksforgeeks.org/support-vector-machine-algorithm/
2. Different Online Sources
3. Link3: https://www.analyticsvidhya.com/blog/2021/10/support-vector-machinessvm-a-complete-guide-for-beginners/
4. Link4: https://medium.com/@davidfagb/understanding-the-support-vector-machine-svm-model-c8eb9bd54a97
   
