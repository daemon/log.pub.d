# Proof Strategies

## General

- Construct an expression that's similar to (or part of) something in the premise, then directly relate it to another.
  - It's often more helpful to use the premise at a later point in the proof, especially if it's a constructive one. For example, you let there be an object, and then at some point you can use the premise to say something about the object.
- A good proof by contradiction can't be easily transformed into a direct proof. It uses the contradiction to derive an alternate reality with extra information, which eventually proves to be incorrect.
- Don't blindly expand the syntax of an expression; instead, focus on its semantics.
  - A corollary is that the equivalent of rubber duck debugging won't get you anywhere.
- Textbook proofs are often too condensed to be informative. Instead, derive the proof yourself.
- Start with the belief that the claim is incorrect, then convince yourself that it's correct.
- Try iteratively refining a proof sketch until it's a rigorous proof, like animation storyboarding. This helps in particular when you're stuck, e.g., going from A to C may be easier than A to B to C, especially if B and C are unknown.
- Thoroughly understand all objects, definitions, theorems, etc., associated with a statement, even if they seem trivial
  - This helps you avoid silly errors and adding too many unnecessary conditions
  - It may also result in a more terse proof
- In general, it is good to learn by counterfactual thinking, always questioning the "what" and "why" of definitions and theorems.
  - Other techniques include spaced repetition (performing recall/reviews right before you forget it, such as first every day, then every two days, then every week, and so on), metacognition (thinking about thought process and where to improve), actually working on proofs, and self-explanation (try to explain each step instead of just reading through a proof)
- Proving that a set has some property is sometimes easier if we construct another set with said quality and prove that the set is a subset of that other set (e.g., the Monotone Class Theorem)
- Stop relying purely on intuition for the final result if you lack experience, since it may rabbithole you into an incorrect solution. Instead, be open-minded and construct things from the ground up.
  - Intuition is still powerful and useful for few-step lookahead if experience is lacking.
- Try to do slot filling more for (possibly complex) algebraic expressions

## Real Analysis

- Knowing every single definition and theorem is important, since the concepts are densely connected.

## Statistics and Probability

- It's clean and helpful to manipulate the expressions coarsely rather than finely, e.g., working directly with the equalities within $Pr(\cdot \leq \cdot)$. 
  - Also proving some V-statistics estimators are biased relative to U-statistics.
- Equivalent forms of distributions (and theorems linking them to some definitions) are often more useful (and simple) toward proving some properties like convergence in distribution.
  - E.g., Levy's continuity Thm., MGF convergence.

- A simple method to generalize proofs is to show some result on the real line and then use isometry to Borel sets.
- One useful application of the Borel-Cantelli theorem, i.e.,

$$\sum_{i=1}^\infty \mathbb{P}(A_i) < \infty \implies \mathbb{P}\left(\bigcap_{m=1}^\infty \bigcup_{i=m}^\infty A_i\right) = 0$$

is to show that $\mathbb{P}(\text{some event infinity often}) = 0$ a.s., e.g.,

$\mathbb{P}(|X_n - X | < \epsilon)$ a.s. for all $\epsilon > 0$.

Here, letting $A_n$ be $|X_n - X | > \epsilon$ be the event and showing that it $= 0$, if we can prove $\sum_{i=1}^\infty \mathbb{P}(A_n) < \infty$, e.g., if the term is something greater than $\frac{1}{n}$ so it's not harmonics (e.g., the infinite series is not divergent).
- It might help to construct a set with some property (e.g., $L = \\{ A  \in \mathcal{F} : \mu(A) = \lambda(A) \\}$ then prove facts about that set to further generalize it (e.g., showing that it's monotone then using the Monotone Class Theorem); see below
<img width="1675" height="721" alt="image" src="https://github.com/user-attachments/assets/5aaf03ed-15ae-4a0a-af84-3c4ae54a2c1f" />


- P-W-Z way of using integration by parts to define a stochastic integral is interesting and easy to digest
