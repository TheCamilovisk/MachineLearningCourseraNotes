# Feature and parameter values
$$
price = w_1x_1 + w_2x_2 + b
$$
- $x_1$: size (feet<sup>2</sup>) -> range: 300 - 2,000 (large)
- $x_2$: # bedrooms -> range 0 - 5 (small)

House: $x_2$ = 2000, $x_2$ = 5, price = $500k
- size of the parameters $w_1$, $w_2$?

# Mean Normalization
Divide fature value by its maximum value and subtract its average value.

# Z-score Normalization
- Compute the standard deviation $\sigma$.
- Subtract the feature's mean from its values
- Divide by $\sigma$.

# Thumbs up rules
- aim for about $-1 \le x_j \le 1$ for each feature $x_j$
	- Rough estimation
	- The range bound should not be too large nor too small