---

# 📘 Mathematical Foundations for Machine Learning

**Read Time:** ~12–15 minutes

This lecture revisits core mathematical concepts from childhood—**vectors, matrices, calculus, and probability**—and explains **why they are critical for Machine Learning (ML)**. These are the building blocks behind algorithms like **linear regression, neural networks, PCA, and backpropagation**.

---

## 1️⃣ VECTORS

### 🔹 What is a Vector?

A **vector** is an ordered list of numbers.

* In **physics**: magnitude + direction
* In **math / ML**: features or data points

In data science, **each data point = a vector**

### 🔹 Types of Vectors

**Row Vector**

```
[2  3]
```

**Column Vector**

```
[2]
[3]
```

---

### 🔹 Example (ML Context)

Suppose we predict exam scores using:

* Study hours
* Sleep hours

Then one student can be represented as:

```
x = (2, 3)
```

Where:

* 2 = study hours
* 3 = sleep hours

This vector lives in **2-dimensional space (R²)**.

---

### 🔹 Vector Addition

Add corresponding elements:

```
A = (2, 3)
B = (1, 4)

A + B = (2+1, 3+4) = (3, 7)
```

✔ Used when combining features or signals.

---

### 🔹 Scalar Multiplication

Multiply vector by a number:

```
2 × (2, 3) = (4, 6)
```

✔ Changes **magnitude**, not direction
✔ Used in **weight scaling**

---

## 2️⃣ MATRICES

### 🔹 What is a Matrix?

A **matrix** is a collection of vectors arranged in rows and columns.

```
A = [1  2]
    [3  4]
```

* Rows = data points
* Columns = features

---

### 🔹 Matrix Dimensions

Written as:

```
rows × columns
```

Example:

```
2 × 2 matrix
```

---

### 🔹 Matrix Multiplication

**Rule:**

> Columns of first matrix = Rows of second matrix

#### Example

```
A = [1  2]   (2×2)
    [3  4]

B = [5]
    [6]     (2×1)
```

Result:

```
A × B = [1×5 + 2×6]
        [3×5 + 4×6]

      = [17]
        [39]
```

✔ Used heavily in:

* Neural networks
* Linear regression
* Image processing

---

## 3️⃣ DOT PRODUCT

### 🔹 What is Dot Product?

Dot product measures **how similar two vectors are**.

Formula:

```
A · B = A₁B₁ + A₂B₂ + ... + AₙBₙ
```

---

### 🔹 Example Calculation

```
A = (2, 3)
B = (4, 1)

A · B = (2×4) + (3×1) = 8 + 3 = 11
```

---

### 🔹 Interpretation

| Dot Product | Meaning                     |
| ----------- | --------------------------- |
| Positive    | Similar direction           |
| Zero        | Perpendicular (no relation) |
| Negative    | Opposite direction          |

---

### 🔹 Cosine Similarity

Formula:

```
cos(θ) = (A · B) / (||A|| ||B||)
```

Range:

```
-1 to +1
```

✔ Used in:

* Recommendation systems
* Search engines
* Vector databases (FAISS, Pinecone)

---

## 4️⃣ EIGENVALUES & EIGENVECTORS

### 🔹 Intuition

When a matrix transforms a vector:

```
A × v = λ × v
```

* **v** = eigenvector (direction unchanged)
* **λ** = eigenvalue (scaling factor)

---

### 🔹 Real-Life Analogy

A **spring**:

* Can stretch or compress
* Direction stays same
* Length changes

---

### 🔹 Example Use: PCA

**Principal Component Analysis (PCA)**:

* Finds directions (eigenvectors)
* With maximum variance
* Reduces dimensions **without losing meaning**

✔ Used in:

* Dimensionality reduction
* Image compression
* Noise removal

✔ Also used in **Google PageRank**

---

## 5️⃣ DIFFERENTIAL CALCULUS

### 🔹 What is Differentiation?

Differentiation measures **change**.

```
dy/dx = rate of change of y w.r.t x
```

---

### 🔹 Example

```
y = 2x
```

Derivative:

```
dy/dx = 2
```

Meaning:

> If x increases by 1 → y increases by 2

---

### 🔹 Graph Meaning

* dy/dx = slope of tangent
* Constant slope → straight line
* Changing slope → curve

✔ Used in:

* Loss minimization
* Optimization

---

## 6️⃣ GRADIENT (MULTIVARIABLE CALCULUS)

### 🔹 Why Gradient?

In ML:

* Output depends on many variables

Example:

```
z = x² + y²
```

---

### 🔹 Partial Derivatives

```
∂z/∂x = 2x
∂z/∂y = 2y
```

Gradient vector:

```
∇z = (2x, 2y)
```

✔ Gradient points in **steepest increase direction**

✔ Used in:

* Gradient Descent
* Neural networks

---

## 7️⃣ CHAIN RULE

### 🔹 What is Chain Rule?

Used when **functions are nested**.

```
y = f(g(x))
```

Derivative:

```
dy/dx = (dy/dg) × (dg/dx)
```

---

### 🔹 Example

```
y = (3x + 1)²
```

Let:

```
g(x) = 3x + 1
y = g²
```

Derivatives:

```
dy/dg = 2g
dg/dx = 3
```

Final:

```
dy/dx = 2(3x + 1) × 3 = 6(3x + 1)
```

---

### 🔹 ML Importance

✔ Core of **Backpropagation**
✔ Used to update weights layer-by-layer
✔ Backbone of deep learning

---

## 🔚 Conclusion

These concepts form the **mathematical spine of Machine Learning**:

| Concept     | Used In              |
| ----------- | -------------------- |
| Vectors     | Features, embeddings |
| Matrices    | Neural networks      |
| Dot Product | Similarity           |
| Eigen       | PCA                  |
| Derivatives | Optimization         |
| Gradient    | Learning             |
| Chain Rule  | Backpropagation      |

📌 **Next Topics Coming Up**

* Linear Regression
* Loss Functions
* Gradient Descent
* Backward Propagation (Deep Dive)

---

