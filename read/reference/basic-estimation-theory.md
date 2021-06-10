# Basic Estimation Theory

We say a parameter $\theta$ of a family of distributions $\mathcal{P}$ is estimable iff
$$
\theta(P) = \mathbb{E}h(X_1, \dots, X_n), \hspace{3mm} X_1, \dots, X_n \sim^{\hspace{-3mm} \text{iid}} P
$$
for all $P \in \mathcal{P}$. The minimum $n$ for this to hold is the degree of $\theta(P)$.

## Sufficient Statistics

A statistic $T(X)$ of a sample $X = \{X_n\}$ is said to be a sufficient statistic for $\theta$ that parameterizes the sample distn. $f(x; \theta)$ iff $f(x; \theta)$ is conditionally independent of $\theta$ given $T(X)$. Intuitively, this definition means that knowing $X$ provides no additional information once $T(X)$ is known.

**Factorization Theorem**: Given continuous or discrete $f(x;\theta)$ and sample $X$, a stastistic $T(X)$ is sufficient iff
$$
f(x;\theta) = g(X)h(\theta, T(X))
$$
for some $g(X)$ and $h(\theta, T(X))$ nonnegative (_Ex_ 1: prove for the discrete case).

**Rao-Blackwell Theorem**: Let there be two estimators of the form $\hat{\theta}_1=f(X)$ and $\hat{\theta}_2 = g(T(X))$, where $T(X)$ is a sufficient statistic of $\theta$ given sample $X=\{X_n\}$. Then $\text{MSE}(\hat{\theta}_1) \geq \text{MSE}(\hat{\theta}_2)$, with unbiasedness being preserved (_Ex_ 2: prove).

