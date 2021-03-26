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
Let's start with writing a scalar function scalar_function, which will apply the following operation with input x and y.

𝑓(𝑥,𝑦)=    𝑥⋅𝑦, if 𝑥≤𝑦
           𝑥/𝑦, else

```python

def scalar_function(x,y):

    if x <= y:
      return x*y
    else:
      return x/y
 ``` 

## 3. Vector function

scalar_function can only handle scalar input, we could use the function np.vectorize() turn it into a vectorized function. Note that the input argument of np.vectorize() should be a scalar function, and the output of np.vectorize() is a new function that can handle vector input.

Please write a vector function vector_function, which will apply the operation 𝑓(𝑥,𝑦) defined above element-wisely with input vectors with same dimension x and y.

```python
def vector_function(x, y):
   
    return np.vectorize(scalar_function)(x,y)
 ``` 
