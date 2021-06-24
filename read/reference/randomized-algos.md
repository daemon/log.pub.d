# Randomized Algorithms

## Useful Inequalities

- $\left(\frac{n}{k}\right)^k \leq \binom{n}{k} \leq \left(\frac{en}{k}\right)^k$ for $k \geq 0$.
- Pascal's Identity: $\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k}$
- Hockey Stick Identity: $\sum_{i=r}^{n} \binom{i}{r} = \binom{n+1}{r+1}$.
- $1-x \leq e^{-x}$, or anything involving exponents.
- Boole's Inequality: $\Pr(\bigcup_{i=1}^n E_i) \leq \sum_{i=1}^n \Pr(E_i)$. Natural consequence of $\sigma$-additivity.
- Jensen's Inequality: $\phi(\mathbb{E}X) \leq \mathbb{E} \phi(X)$ for convex $\phi$, with strict inequality for strictly convex $\phi$ and nondegenerate $F_X(x)$.
- Markov's Inequality: $\Pr(Y \geq t) \leq \frac{\mathbb{E}Y}{t}$ for $Y, t$ non-negative. Prove by defining dummy variable $f(y) = 1$ if $y \geq t$, $0$ otherwise, then taking expectation over that.
  - Only really useful for deriving other inequalities. Sharpest bound possible given only non-negativity.
- Chebyshev's Inequality: $\Pr(|X - \mu| \geq t\sigma) \leq \frac{1}{t^2}$. Prove by considering the square of both sides in the probability.