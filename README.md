# -Support-Vector-Machine
#Binary Classification  #Nominal Classification #Ordinal Classification # Nonlinear SVM

# Goal of SVM
The goal of an SVM (Support Vector Machine) model is to separate datasets into distinct classes by finding the **Maximum Marginal Hyperplane (MMH)** in a multidimensional space. This hyperplane is determined iteratively to minimize error, effectively dividing the data into clearly defined classes.

# What are the Support Vectors?
- Given a hyperplane, the support vectors are observations that are nearest to the hyperplane.
- Change the hyperplane, get a different set of support vectors
- They are the observations that have a high tendency to be misclassified.
- They have direct and often the highest influence on the weights (i.e., 𝑤_1,…,𝑤_𝑝)  of the hyperplane.

# The Optimal Linear Separator
- SVM finds an optimal choice of 𝑤_1, 𝑤_2, and 𝑐 such that it **maximizes the margin between the hyperplane and the support vectors.**
- As you can see, the hyperplane is fully specified by the support vectors and all other training observations are ignorable.

<img width="480" alt="image" src="https://github.com/ColleenJung/-Support-Vector-Machine/assets/119357849/05053453-84c6-45a9-ad65-f8e551af4733">

# The sklearn.svm.LinearSVC() Function
- Since the number of observations is usually greater than the number of features, we set **dual = False** per documentation advice.
- Although dual = False does not use random numbers, we still set **random_state** to a positive integer just in case.
- The Intercept 𝑤_0  value can be retrieved from the **intercept_**object
- The array of coefficients 𝐰 can be retrieved from the **coef_** object
- The hyperplane is constructed from the equation 𝑤_0+𝐰^𝑡 𝐱=𝟎

# Example datasets
1. A Simple Binary Classification
2. Feature Selection
3. Nominal Classification
4. Ordinal Classification
5. An Example of Nonlinear Support Vector Machine
















