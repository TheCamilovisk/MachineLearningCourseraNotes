Some function
$$
J(w, b)
$$
Want
$$
\underset{w, b}{min}J(w, b)
$$
## Outline (downhill)
- Start with some $w,b$ (set $w=0, b=0$)
- Keep changing $w,b$ to reduce $J(w,b)$
- Until we settle at or near a minimum (local)
	- May have more than 1 minimum if not:
		- squared error cost
		- linear regression

## Algorithm

1. 
$$
w = w - \alpha \frac{\delta}{\delta w}J(w,b)
$$
$$
b = b - \alpha \frac{\delta}{\delta b}J(w,b)
$$
- $\alpha$: learning rate
- $\frac{\delta}{\delta w}J(w,b)$: Derivative
Simulataneously update $w$ and $b$.

# Intuition

$$
J(w)
$$
$$
w = w - \alpha \frac{\delta}{\delta w}J(w)
$$
$$
\underset{w}{min}J(w)
$$
- If $\alpha$ is too small -> gradient descent may be slow
- If $\alpha$ is too large ->
	- Overshoot, neve reach minimum
	- Fail ro converge, diverge

Near a local minimum
- Derivative becomes smaller
- Update steps become smaller

## Batch gradient descent

Each step of gradient descent uses all the training examples