## Parameters and features

- $\vec{w}$ = $[w_1 \quad w_2 \quad w_3]$
- $b$ is a number
- $\vec{x}$ = $[x_1 \quad x_2 \quad x_3]$
- linear algebra: count from 1
- numpy: count from 0

### Without vectorization
$$
f_{\vec{w},b}(\vec{x}) = \sum_{j=1}^n w_jx_j + b
$$
### Vectorization
$$
f_{\vec{w},b}(\vec{x}) = \vec{w}\cdot\vec{x} + b
$$
## Gradient Descent
$n$ features ($n \ge 2$)
repeat:
$$
w_n = w_n - \alpha\frac{1}{m} \sum_{i = 1}^m (f_{\vec{w}, b}(\vec{x}^{(i)}) - y^{(i)})x_n^{(i)}
$$
$$
b = b - \alpha\frac{1}{m} \sum_{i = 1}^m (f_{\vec{w}, b}(\vec{x}^{(i)}) - y^{(i)})
$$
simultaneously update $w_j$ (for $j=1, \dots, n$) and $b$

## Alternative way
### Normal equation
- Only fr linear regression
- Solve for $w,b$ without iterations
#### Disadvantages
- Doesn't generalize to other learning algorithms
- Slow when number of features is large (> 10000)
### What you need to know
- Normal equation method may be used in machine learning libraries that implement linear regression
- Gradient descent is the recommended method for finding parameters $w,b$.
