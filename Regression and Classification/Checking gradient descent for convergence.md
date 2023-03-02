- Check the cost x iteration graph (learning curve $J(\vec{w}, b$))
- $J(\vec{w}, b)$ should decrease after every iteration
- Iteration needed varies
## Automatic convergence test
- Let $\epsilon$ be $10^{-3}$
- If $J(\vec{w}, b)$ decreases by $\le \epsilon$ in one iteration, declare convergence (close to global minimum)

## Identify problem with gradient descent
- If the learning curve is bouncing up and down, maybe the code is buggy or the learning rate is too large
- Values of $\alpha$ to try: $[\cdots, 0.001, 0.01, 0.1, 1, \cdots]$.