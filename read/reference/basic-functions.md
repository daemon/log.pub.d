# Basic Function Geometry

Basic continuity and geometric properties:

**Convex**: $f(x)$ is convex iff $\forall u, v \in \Omega. f(u) \geq f(v) + \langle u-v, \nabla f(v) \rangle$. If the inequality is strict, then it's strictly convex.

**Strongly convex**: $f(x)$ is $m$-strongly convex iff $\forall u, v \in \Omega. f(u) \geq f(v) + \langle u-v, \nabla f(v)\rangle + \frac{m}{2}\lVert u-v \rVert^2$. It bends more strongly than some quadratic times an $m$.

**Lipschitz**: $f(x)$ is $L$-Lipschitz iff $\lVert \nabla f(x) \rVert \leq L \iff \lVert f(u) - f(v) \rVert \leq L \lVert u - v \rVert$.

**Smoothness**: $f(x)$ is $\beta$-smooth if its gradient is $\beta$-Lipschitz, i.e., $\lVert \nabla f(u) - \nabla f(v) \rVert \leq \beta\lVert u-v\rVert \iff f(u) \leq  f(u) + \frac{\beta}{2} \lVert u-v \rVert^2$.

## Gradient Descent Bounds

If $f(x)$ is $L$-Lipschitz, 

