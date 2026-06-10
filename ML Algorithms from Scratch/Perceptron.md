# Perceptron

1. `__init__`
   It is a constructor that initializes the class variables for lr(learning rate) and epochs(no. of iterations to run).

2. `fit`
    - Initalizes the weights with 0's and bias with 0
    - Ioops for *epochs* times
    - $zip$ function combines the two iterables *X* and *y*
    - For each *xi* it predicts it's corresponding y value.
    - Calculates $lr * (y - \hat y)$
    - Updates the weights and biases accordingly

### LR
- Stands for *Learning Rate*
- It controls how much the perceptron adjusts its weights after each mistake
- A larget learning rate makes bigger updates; a smaller one makes slower, more stable updates.
- Update rule uses it directly:
  $w = w + lr * (y - \hat y) * x$
- 