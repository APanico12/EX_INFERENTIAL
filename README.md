Statistical inference exercises

# Excercise 2.9 Wasserman

In this exercise, we aim to estimate tau_hat through simulation. Specifically, our simulation is based on generating 10 random values from a uniform distribution and repeating the process 10^6 times. For each simulation, we take the maximum and minimum values as estimates for a_hat and b_hat, respectively. Using these, we calculate tau_hat and obtain a distribution of this estimator. Finally, we compute the Mean Squared Error (MSE) as:

MSE = E[(tau_hat - tau)^2]

where tau is the expected value of the uniform distribution Uniform(1, 3).


# Excercise 7.3 Casella Berger

Estimation of Gamma Distribution Parameters

This program calculates the parameters  \alpha (shape) and \beta (inverse scale) of a **gamma distribution** using the **Maximum Likelihood Estimation (MLE)** technique. 
In particular, the parameter \( \alpha \) is determined numerically using the **Newton's method**, and \( \beta \) is subsequently calculated using a direct relationship.

## Newton's Method

Newton's method is a numerical algorithm used to find the zeros of a function. In this program, it is applied to find the zero of the derivative of the log-likelihood function with respect to the parameter \( \alpha \). 
Starting from an initial estimate, \( \alpha_0 \), the method iteratively updates the solution using the formula:

\[ \alpha_{n+1} = \alpha_n - \frac{f(\alpha_n)}{f'(\alpha_n)} \]

where:
- \( f(\alpha) \) is the derivative of the log-likelihood function with respect to \( \alpha \).
- \( f'(\alpha) \) is the second derivative of the log-likelihood function.

This technique is chosen for its efficiency and rapid convergence, especially in well-conditioned problems like the one addressed in this script.
