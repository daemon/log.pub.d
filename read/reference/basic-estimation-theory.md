# Basic Estimation Theory

We say a parameter $\theta$ of a family of distributions $\mathcal{P}$ is estimable iff
$$
\theta(P) = \mathbb{E}h(X_1, \dots, X_n), \hspace{3mm} X_1, \dots, X_n \sim^{\hspace{-3mm} \text{iid}} P
$$
for all $P \in \mathcal{P}$. The minimum $n$ for this to hold is the degree of $\theta(P)$.

## Sufficient Statistics

A statistic $T(x)$ of a sample $X = \{X_n\}$ is said to be a sufficient statistic for $\theta$ that parameterizes the pdf $f(x; \theta)$ iff $f(x; \theta)$ is conditionally independent of $\theta$ given $T(x)$, i.e., $f(x | t; \theta) = g(x)$. Intuitively, this definition means that knowing $X$ provides no additional information about $\theta$ once $T(x)$ is known.

**Factorization Theorem**: Given continuous or discrete $f(x;\theta)$ and sample $X$, a statistic $T(X)$ is sufficient iff
$$
f(x;\theta) = g(x)h(\theta, T(x))
$$
for some $g(x)$ and $h(\theta, T(x))$ nonnegative (_Ex_ 1: prove for the discrete case; soln: $f(x; \theta) = f(x, t; \theta)$ and chain rule).

**Rao-Blackwell Theorem**: Let there be two estimators of the form $\hat{\theta}_1=f(X)$ and $\hat{\theta}_2 = \mathbb{E}[\hat{\theta}_1|T]$, where $T(X)$ is a sufficient statistic of $\theta$ given sample $X=\{X_n\}$. Then $\text{MSE}(\hat{\theta}_2) \leq \text{MSE}(\hat{\theta}_1)$, with unbiasedness being preserved (_Ex_ 2: prove; soln: start with the left side, condition on $T$, then use Jensen's Inequality).

