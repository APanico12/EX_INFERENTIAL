Statistical inference exercises

Excercise 2.9 Wasserman
In this exercise, we aim to estimate tau_hat through simulation. Specifically, our simulation is based on generating 10 random values from a uniform distribution and repeating the process 10^6 times. For each simulation, we take the maximum and minimum values as estimates for a_hat and b_hat, respectively. Using these, we calculate tau_hat and obtain a distribution of this estimator. Finally, we compute the Mean Squared Error (MSE) as:

MSE = E[(tau_hat - tau)^2]

where tau is the expected value of the uniform distribution Uniform(1, 3).