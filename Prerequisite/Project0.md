## 1. Neural Network


Here, we will write a function neural_network, which will apply a neural network operation with 2 inputs and 1 output and a given weight matrix.

```python
def neural_network(inputs,weights):

  wT = np.transpose(weights)
  product = np.matmul(wT,inputs)
  out = np.tanh(product)
  return(out)
```

## 2. Vectorize function


