# Calculus for Data Science & Machine Learning

Calculus is essential for understanding how machine learning models learn, optimize loss functions, and update parameters. It explains **how parameters change**, **how errors are minimized**, and **how models converge**.

---

## 1. Differentiation
- Measures the rate of change of a function  
- Shows how model output changes with respect to parameters  
- Foundation for optimization algorithms  
- Used to compute slopes and gradients  

**ML Usage:**  
Used to understand how changing weights affects prediction error.

---

## 2. Partial Derivatives
- Differentiation of multivariable functions  
- Partial derivative w.r.t. one variable while keeping others constant  
- Geometric interpretation of slopes in higher dimensions  
- Core component of gradient computation  

**ML Usage:**  
Used to compute gradients for models with multiple parameters.

---

## 3. Functions of Multiple Variables
- Multivariable functions  
- Limits of multivariable functions  
- Continuity in higher dimensions  
- Partial derivatives in multivariable settings  

**ML Usage:**  
Loss functions depend on many parameters simultaneously.

---

## 4. Integrations
- Indefinite integrals  
- Definite integrals  
- Properties of integration  

**Applications in Data Science:**  
- Probability Density Functions (PDF)  
- Cumulative Distribution Functions (CDF)  
- Expectation and variance  

---

## 5. Beta and Gamma Functions
- Gamma function definition and properties  
- Beta function definition  
- Relationship between Beta and Gamma functions  

**Applications:**  
- Beta distribution  
- Dirichlet distribution  
- Bayesian statistics  

---

## 6. Minima and Maxima
- Local minima and maxima  
- Global minima and maxima  
- First derivative test  
- Second derivative test  
- Convex vs non-convex functions  

**ML Usage:**  
Training models means finding the **minimum loss**.

---

## 7. Loss Functions
- Purpose of a loss function  
- Measures prediction error  

### Regression Loss Functions
- Mean Squared Error (MSE)  
- Mean Absolute Error (MAE)  

### Classification Loss Functions
- Log Loss  
- Cross-Entropy Loss  

**Role:**  
Guides the optimization process during training.

---

## 8. Gradient Descent
- Core optimization algorithm  
- Moves parameters in the direction of minimum loss  

### Variants of Optimizers
- Batch Gradient Descent  
- Stochastic Gradient Descent (SGD)  
- Mini-batch Gradient Descent  
- Momentum  
- RMSProp  
- Adam Optimizer  

**ML Usage:**  
Used to iteratively update weights.

---

## 9. Chain Rule
- Differentiation of composite functions  
- Backbone of backpropagation  

**ML Usage:**  
Allows gradients to flow through neural network layers.

---

## 10. Backpropagation
- Algorithm for training neural networks  
- Uses chain rule to compute gradients  
- Updates weights and biases layer by layer  

**Importance:**  
Essential for deep learning.

---

## 11. Jacobian and Hessian Matrices
- Jacobian: first-order partial derivatives matrix  
- Hessian: second-order partial derivatives matrix  

**Usage:**  
- Gradient mapping  
- Second-order optimization  
- Curvature analysis  

---

## 12. Higher-Order Derivatives
- Second and higher derivatives  
- Captures curvature of loss functions  

**ML Usage:**  
Helps analyze convergence speed and stability.

---

## 13. Taylor’s Series
- Approximates complex functions using polynomials  
- Simplifies non-linear functions near a point  

**ML Usage:**  
Used in optimization theory and numerical methods.

---

## 14. Fourier Transformations
- Converts data from time domain to frequency domain  

**Applications:**  
- Signal processing  
- Image processing  
- Feature extraction  

---

## 15. Area Under the Curve (AUC)
- Area under ROC curve  

**ML Usage:**  
- Model evaluation metric  
- Measures classification performance  

---

## Summary

Calculus forms the mathematical backbone of machine learning.  
It enables:
- Optimization of models  
- Learning through gradients  
- Efficient convergence  
- Reliable performance evaluation  

A strong understanding of these concepts is critical for mastering Data Science and Machine Learning.
