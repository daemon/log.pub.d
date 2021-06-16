# Fairness in Deep Learning

Fairness-enforcing methods minimize interattribute differences in the model predictions, where each attribute corresponds to some relevant subgroup within the input distribution. For example, in speech recognition, two possible subgroups are African American Vernacular English (AAVE) and non-AAVE. To improve social equity, we seek to minimize any differences in model quality between the two groups.

Concretely, given a model $f(\cdot; \theta)$ and training data $\{(X_i, A_i, Y_i)\}$ indexed by $i \in \mathcal{I}_\text{training}$, we want to learn a model $f(\cdot; \theta^*)$ such that $\hat{Y} = f(X; \theta^*)$ is conditionally independent of the attribute $A$ given the prediction $Y$.

## Discrete Approach #1 (State of the Art)

Romano et al. [1] describe an adversarial approach 