
## Randomization

1. Write a function called randomization that takes as input a positive integer n, and returns A, a random n x 1 Numpy array.

```python
def randonization(n):

  A = np.random.random([n,1])
  return A
```

## Operations

2. Write a function called operations that takes as input two positive integers h and w, makes two random matrices A and B, of size h x w, and returns A,B, and s, the sum of A and B.

```python
def operations(h,w):

  A = np.randon.random([h,w])
  B = np.random.random([h,w])
  s = A + B
  return A,B,s
```

## Norm

3. Write a function called norm that takes as input two Numpy column arrays A and B, adds them, and returns s, the L2 norm of their sum.

```python
def norm(A,B):

  s = A + B
  n = np.linalg.norm(s)
  return n
```
