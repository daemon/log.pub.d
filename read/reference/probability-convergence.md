# Convergence in Probability Theory

Convergence in probability theory deals with a sequence of RVs approaching an RV in the limit.

**Convergence in distribution**. Pointwise equality between the CDF of the nth r.v. in a sequence X1, ..., Xn as n goes to infinity:
$$
\lim_{n\to \infty} F_n(x) = F(x),
$$
where F(x) is the CDF of X. We write
$$
X_n \to^\mathcal{\hspace{-4mm}D} X
$$
The continuous mapping theorem (i.e., for a sequence of RVs {Xn} converging to some RV X, continuous functions of Xn also converge to the same function of X) and Levy's continuity theorem (convergence in distribution iff characteristic functions converge pointwise) are useful.

**Convergence in probability**. The probability of Xn being outside of the ball of radius epsilon centered at X approaches zero for any epsilon, i.e.,
$$
\lim_{n\to \infty} \Pr(| X_n - X | > \epsilon)= 0.
$$
 The continuous mapping theorem holds as well.

**Almost sure convergence**. The probability of Xn = X approaches one:
$$
Pr(\lim_{n \to \infty} X_n = X) = 1.
$$
If we disregard sets of measure zero (i.e., which sure convergence covers), this is the strongest form of convergence. Practically, this form is the strongest: A.S. implies conv. in P implies conv. in D.

## Applications

- A method to make a statement about a sequence of RVs is to transform them into their characteristic functions (projection onto Fourier basis), expand using Taylor's theorem, drop off the unimportant terms, and then use Levy's continuity theorem to show convergence in distribution (see proof of the classical CLT).
- CLT itself clearly useful for asymptotics for everything.
- Slutsky's Thm. deals with additions and products of Xn and Yn converging in distn to cX, X + c, and X/c if Xn and Yn converge in probability to X and constant c, respectively.

