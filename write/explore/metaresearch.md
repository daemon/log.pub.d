# Meta-research Notes

My research follows these rules, with ideas and feedback from Jimmy Lin and his research group. As usual, feedback does not imply endorsement. Be sure to read [his guide](https://github.com/lintool/guide) if you haven't already.

## Writing Style

1. **Justify every claim and choice by argument**, which takes on one (or more) of the following types, in decreasing order of strength:
   1. Deduction from first principles (e.g., mathematical proof).
   2. Inductive and abductive reasoning (e.g., strong experimental evidence).
   3. Literature (e.g., following X et al.).
   4. Bandwagoning (e.g., everybody uses this model).
   5. Authority (e.g., Google did it).
   6. Personal anecdote (e.g., our preliminary runs show this but no data given).
2. **Use plain syntax.** Readers are here to admire the problem and the solutions, not the prose.
3. **Use fun semantics.** Make the problem and the solutions interesting.
4. **Give simple yet intriguing specific examples.** Defer the general case for later (or place in the appendix if advisable). Readers' attention falls off quickly, and it's important to capture that for as long as possible. A specific case of your problem allows them to immediately taste what you're trying to solve, without the complexities of the general case. For example,
   - Bad: "Let there be a parametric, differentiable classifier $f(x; \theta)$ parameterized by (a possibly infinite number of parameters) $\theta$ over the set of reals. Let there be a generative model $g(x; \phi)$ for the nondegenerate data probability distribution $p(x)$ where ..."
   - Good: "Consider the specific text classification task, with a classification model $f(x)$ and a language model $g(x)$."
5. **Lighten the cognitive load** of the reader as much as possible. A good paper uses the least number of neurons as possible to defend itself.
6. **Use the background and related work section to frame the problem and your solution.** The introduction describes the problem, and the methods section solves it. To bridge the two, the background and related work part explains why it's hard and the shortcomings of previous work.

## Experimental Style

1. **Pick a problem that satisfies the following properties:** 
   1. **Impactful**: work on something that matters to many; [research isn't done in a vacuum](https://www.goodreads.com/en/book/show/15731248-the-ph-d-grind). Always consider the implications of your claims and findings.
   2. **Interesting**: work on something that matters to you. If you don't care about the success of a project, you won't realize your potential.
   3. **Realistic**: [work on something just outside your reach](https://terrytao.wordpress.com/career-advice/continually-aim-just-beyond-your-current-range/). That way, you continually grow your realm of competence.
   4. **Capturable**: work on something whose solution's value you can capture better than others. [It's about the size of the bite, not the size of the cake](https://www.amazon.com/Zero-One-Notes-Startups-Future/dp/0804139296).
   
2. **Pick a hypothesis that satisfies the following properties:**

   1. **Falsifiable**: a hypothesis is _not_ a mere statement of fact. It is a claim that you need to support with the aforementioned argument types.
   2. **Concrete**: the wording of the hypothesis must be precise. It must leave no room for misinterpretation, as it's the centerpiece of the paper.
   3. **Explainable**: ideally, the hypothesis has an explanatory clause following it, which provides critical understanding and insight.

   Here are some examples:

   - Terrible: "BERT is sometimes prunable and other times not." (unfalsifiable, vague, and unimpactful)
   - Bad: "BERT achieves a compression ratio of 10.5 on the SST-2 dataset." (unfalsifiable)
   - Okay: "BERT achieves a higher pruning compression ratio on tasks with shorter sentences than it was pretrained on."
   - Good: "Pretrained transformers achieve higher compression ratios on tasks with shorter sentences than they were pretrained on, because the class token attends to fewer tokens, reducing the parameter need."

3. **Identify critical points early.** Which potential finding, if discovered, would result in a waste of time and effort? For example,

   1. Is my task important and my approach new? Do literature search before novel design.
   2. Would baselines outperform my approach? Do baselines before novel methods.
   3. Is this task beyond my current resources? Do planning before execution.

4. **Be flexible.** If a story isn't working, improve it. If a project no longer excites you, end it. You definitely won't excite the reader, who might not be excited _even when_ you are excited. Further, you won't care if it gets published, and academia isn't driven by prestige or wealth. Those are byproducts of solving interesting problems.

5. **Avoid security through obscurity.** If your design has a potential flaw, you must either explicitly justify it or change it. It's unethical and wasteful to mislead yourself and others.

6. **Get feedback early and often.** Talk to your supervisor. Talk to your friends. Talk to your mother and her cat. Again, [research isn't done in a vacuum](https://www.goodreads.com/en/book/show/15731248-the-ph-d-grind), and [diversity matters](https://hbr.org/2017/03/teams-solve-problems-faster-when-theyre-more-cognitively-diverse).