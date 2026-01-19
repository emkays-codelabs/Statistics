# 📘 Hypothesis Testing and T-Test

---

## 1️⃣ Measures of Central Tendency  

These describe the **center** of data.

### Mean (Average)  
Mean = (Sum of all values) / Number of values  

Example:  
60, 70, 80  
Mean = (60 + 70 + 80) / 3 = 70  

### Median  
Middle value when data is ordered.  
60, 70, 80 → Median = 70  

### Mode  
Most frequent value.  
60, 70, 70, 80 → Mode = 70  

---

## 2️⃣ Skewness (Shape of Data)

**Skewness** describes the **shape of a dataset** and shows how the data is **distributed around the mean**.

It tells us whether the data is:
- Balanced  
- Pulled to the right  
- Pulled to the left  

Understanding skewness helps us interpret **averages**, choose the **right statistical test**, and understand **real-world data patterns**.

![Skewness Diagram](skewness.png)

### 🔹 1. Symmetric Distribution  
- Mean = Median = Mode  
- Balanced shape  
- No skew  

### 🔹 2. Positively Skewed (Right-Skewed)  
- Mean > Median > Mode  
- Few very large values pull the mean right  

### 🔹 3. Negatively Skewed (Left-Skewed)  
- Mean < Median < Mode  
- Few very small values pull the mean left  

---

## 3️⃣ Normal Distribution  

A **bell-shaped curve** 🔔  
Mean = Median = Mode  

### 68–95–99.7 Rule

| Range | % of Data |
|-------|-----------|
| μ ± 1σ | 68% |
| μ ± 2σ | 95% |
| μ ± 3σ | 99.7% |

Example:  
If mean = 70, SD = 10  
68% of scores are between 60 and 80  

![Normal Distribution](Normal_distribution.png)

---

## 6️⃣ What is a Hypothesis?

A **hypothesis** is a statement about a population.

Example:  
"The average score is 70."

---

## 7️⃣ Hypothesis Testing Steps

1. State H₀ and H₁  
2. Choose test  
3. Calculate statistic  
4. Find p-value  
5. Make conclusion  

---

## 8️⃣ Null Hypothesis (H₀)

H₀ = No change / no effect  

Example:  
H₀: μ = 70  

---

## 9️⃣ Alternative Hypothesis (H₁)

| Type | Meaning |
|------|---------|
| μ ≠ 70 | Two-tailed |
| μ > 70 | Right-tailed |
| μ < 70 | Left-tailed |

---

# 🔟 Significance Level and Confidence Level

## The Formula  
C + α = 1  

Where:  
- α = Significance Level  
- C = Confidence Level  

---

### 10.1 Significance Level (α)

α is the **risk of rejecting a true null hypothesis**.

Common values:

| α | Meaning |
|----|--------|
| 0.05 | 5% risk |
| 0.01 | 1% risk |

---

### 10.2 Confidence Level (C)

C tells how confident you are in your result.

| C | Meaning |
|----|--------|
| 0.95 | 95% confident |
| 0.99 | 99% confident |

---

### 10.3 Why C + α = 1?

Example:  
α = 0.05  
C = 0.95  

0.95 + 0.05 = 1  

Meaning:  
95% confidence, 5% risk of error.

---

## 4️⃣ Z-Score  

A **Z-score** measures how far a value is from the mean in terms of **standard deviations**.

Formula:  
Z = (X − μ) / σ  

Example:  
Score = 80  
Mean = 70  
SD = 5  

Z = (80 − 70) / 5 = 2  

Meaning:  
The score is **2 SD above** the mean.

---

## 5️⃣ Z-Table (Standard Normal Table)

A **Z-table** shows the probability (area) to the **left** of a Z-score.

| Z-value | Meaning | Area to the Left |
|--------|---------|------------------|
| 0.00 | At the mean | 0.5000 |
| 1.00 | 1 SD above | 0.8413 |
| 1.64 | Top 5% | 0.9500 |
| 1.96 | Top 2.5% | 0.9750 |
| 2.33 | Top 1% | 0.9900 |

How to read:
1. Row = first two digits  
2. Column = decimal  
3. Cell = area to the left  

Example:  
Z = 1.23 → Area ≈ 0.8907  

---

## 1️⃣1️⃣ P-Value  

The p-value shows how likely the result is **if H₀ is true**.

| p-value | Decision |
|----------|----------|
| p ≤ α | Reject H₀ |
| p > α | Do not reject H₀ |

---

## 1️⃣2️⃣ Z-Test (Large Sample, σ Known)

Z = (x̄ − μ) / (σ / √n)

Example:  
μ = 500  
x̄ = 495  
σ = 10  
n = 36  

Z ≈ −3  
p ≈ 0.0026  

Conclusion:  
Reject H₀  
Bottles are underfilled.

---

## 1️⃣3️⃣ One-Sample T-Test  

Used when:  
- n < 30  
- σ unknown  

Example:  
Mean = 72  
SD ≈ 5.87  

t ≈ 0.76  
df = 4  

Conclusion:  
Do not reject H₀

---

## 1️⃣4️⃣ Independent T-Test  

Compare two groups.

p = 0.03  

Conclusion:  
Reject H₀  
Groups are different.

---

## 1️⃣5️⃣ Paired T-Test  

Before vs After  
p = 0.01  

Conclusion:  
Training improved performance.

---

## 1️⃣6️⃣ T-Table (α = 0.05)

| df | t |
|----|----|
| 1 | 12.706 |
| 2 | 4.303 |
| 3 | 3.182 |
| 4 | 2.776 |
| 5 | 2.571 |
| 10 | 2.228 |
| ∞ | 1.960 |

---

## 1️⃣7️⃣ Chi-Square Test  

Used for categorical data.

Conclusion:  
The die is fair.

---

## 1️⃣8️⃣ Chi-Square (Independence)  

Conclusion:  
Preference depends on gender.

---

## 1️⃣9️⃣ ANOVA  

Used for 3+ groups.

Conclusion:  
At least one group differs.

---

## 2️⃣0️⃣ When to Use Each Test

| Situation | Test |
|----------|------|
| Large n, σ known | Z-test |
| Small n | T-test |
| Two groups | Independent T |
| Before/After | Paired T |
| Categorical | Chi-square |
| 3+ groups | ANOVA |

---

## 2️⃣1️⃣ Final Exam Summary  

- H₀ = No effect  
- H₁ = There is an effect  
- α = Significance level  
- p-value = Evidence strength  
- Reject H₀ = Significant  

---
