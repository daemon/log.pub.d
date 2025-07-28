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

## Real Analysis

- Knowing every single definition and theorem is important, since the concepts are densely connected.

## Statistics and Probability

- It's clean and helpful to manipulate the expressions coarsely rather than finely, e.g., working directly with the equalities within $Pr(\cdot \leq \cdot)$. 
  - Also proving some V-statistics estimators are biased relative to U-statistics.
- Equivalent forms of distributions (and theorems linking them to some definitions) are often more useful (and simple) toward proving some properties like convergence in distribution.
  - E.g., Levy's continuity Thm., MGF convergence.

- A simple method to generalize proofs is to show some result on the real line and then use isometry to Borel sets.
