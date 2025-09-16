# Function Optimization

In this project, we aim to **optimize a 3-dimensional function** defined as:

f(x1, x2) = 100 * (x1 - x2^2)^2 + (1 - x2)^2


---

## ⚙️ Optimization Methods Used

### 1. Steepest Descent
- Also known as **Gradient Descent**, this method iteratively moves in the direction of the **negative gradient** of the function.  
- The step size (learning rate) determines how far we move in each iteration.  
- Simple to implement, but may converge slowly near the optimum.

### 2. Newton's Method
- Uses **second-order derivatives (Hessian matrix)** to estimate curvature of the function.  
- Updates are calculated using both gradient and curvature, allowing **faster convergence** than gradient descent in many cases.  
- Computationally more expensive due to Hessian calculation.

### 3. One-Step Newton
- A variation of Newton's method where only **one update step** is applied using the gradient and Hessian at the initial point.  
- Provides a good approximation of the optimum quickly if the function is well-behaved near the starting point.

---

## 🎯 Conclusion
Among the methods tested, **One-Step Newton** reached a point **closer to the true optimum** of the function compared to the others, demonstrating its efficiency for well-conditioned problems.
