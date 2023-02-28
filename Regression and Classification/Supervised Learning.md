$$
\text{Input} \rightarrow \text{output label}
$$
- Learns from being given "right answers"

|Input (X)|Output (Y)|Application|
|:---:|:---:|:---:|
|email|spam? (0/1)|spam filtering|
|audio|text transcripts|speech recognition|
|English|Spanish|machine translation|
|ad, user info|click? (0/1)|online advertising|
|image, radar info|position of other cars|self-driving car|
|image of phone|defect? (0/1)|visual inspection|

## Regression
- Predict a **number**
- **Infinitely** many possible outputs
## Classification
- Predict **categories**
- **Small number** of possible outputs

## Cost Function
### Model
$$
f_{w, b}(x) = wx + b
$$
$w,b$ : parameters / coefficients / weights 

Find $w, b$: $\hat{y}^{(i)}$ is close to $y^(i)$ for all $(x^{(i)}, y^{(i)})$.

**Squared error cost function**
$$
J(w, b) = \frac{1}{2m} \sum^m_{i=1} (f_{w, b}(x^{(i)}) - y^{(i)})^2
$$
$m$: number of training samples

### Goal
$$
\underset{w, b}{minimize} = J(w, b)
$$
