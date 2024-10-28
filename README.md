java c
Midterm IEOR E4525 Fall 2023 
October 22, 2024
1 Kernel-based Nearest Neighbor Regression [20 points] 
Consider a kernel K(x, x′) that measures the similarity between two points x and x′. We have the following model:

where (xi, yi)i∈[n]represents the training data. Assume that K is a symmetric and non-negative function.
In the first three parts, we consider the tricubic kernel which is given by

Let ∥x − x′∥ = d, and consider K(d) in the first two parts.
1. Is the kernel K(d) continuous in d? Is it differentiable in d? [6 points]
2. Is the kernel K(d) monotonic in d? [3 points]
3. Describe the region of x around a fixed point x0 for which K(x, x0) = 8/1. [3 points]
4. Is it possible to have an kernel K(x, x′) (independent of the dataset) which mimics 1-NN? If yes, which one? If not, give an example to disprove it. [4 points]
5. Is it possible to have a kernel K(x, x′) (independent of the dataset) which mimics n-NN? If yes, which one? If not, give an example to disprove it. [4 points]
2 Logistic Regression [10 points] 
Let us use the following models of logistic regression for a binary classification with a sigmoid function g(z) = 1+e−z/1.
• Model A: P(Y = 1|X, w1, w2) = g(w1X1 + w2X2)
• Model B: P(Y = 1|X, w1, w2) = g(w0 + w1X1 + w2X2)
The dataset has three training examples.

1. Does it matter how the third example is labelled in Model A? That is, would the learned value of w = (w1, w2) be different if we change the label of the third example to −1? Does it matter for Model B? Explain the answers. (Hint: think of the decision boundary on 2D plane. Also, if the output is more than or equal to 0.5, then it is classified as 1 and -1 otherwise.) [5 points]
2. Suppose we train the logistic regression model (Model B) based on the n training examples x(1), . . . , x(n) and labels y(1), . . . , y(n) by maximizing the penal代 写Midterm IEOR E4525 Fall 2023Java
代做程序编程语言ized log-likelihood of the labels:

For large λ, the log-likelihood terms will behave as linear functions of w.

Express the penalized log-likelihood using this approximation (with Model A), and derive the expression for MLE ˆw in terms of λ and training data {x(i), y(i)}. Based on this, explain how w behaves as λ increases. (Assume that each x(i) = (x(1i)x(2i))T and y(i) ∈ {−1, +1}) [5 points]
3 Naive Bayes [25 points] 
Consider the following training data with binary features L, M, N in {0, 1}, and binary class C in {0, 1}:

1. Is Naive Bayes generative or discriminative? Explain. [4 points]
2. Compute the following conditional probabilities: P(L = 0|C = 1), P(M = 1|C = 1), P(N = 1|C = 1), P(L = 0|C = 0), P(M = 1|C = 0), P(N = 1|C = 0). [6 points]
3. Predict the class label for (L = 0, M = 1, N = 1) using Naive Bayes. [5 points]
4. Are the variables L and M independent in the training data? [5 points]
5. Are the variables L and M conditionally independent in the training data given that C = 1? [5 points]
4 Bootstrapping and LOO Cross-Validation [15 points] 
1. Consider that there are n iid random variables (Xi)i∈[n] with mean µ and variance σ2. Let (Xi∗)i∈[m] be a bootstrap sample of size m with mean ¯X∗ =Pmi=1 m/X∗i.
Compute E(X¯ ∗|X1, . . . , Xn), Var(X¯ ∗|X1, . . . , Xn), E(X¯ ∗), and Var(X¯ ∗) [10 points]
2. Leave-one-out (LOO) cross-validation is an extreme form. of k-fold cross-validation, where we train our machine-learning model n times where n is our dataset’s size. Each time, only one (different every time) sample is used as a test set while the rest are used to train our model. The error is then calculated by averaging over these n errors. Draw a 2D dataset where 1-nearest neighbor (1-NN) has a lower LOO cross-validation error than SVM. [5 points]









         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
