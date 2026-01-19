# One-Sample t-Test: Complete Explanation with Applications

## 1. Introduction

A **t-test** is a statistical method used to determine whether the mean of a sample is significantly different from a claimed population mean when the population standard deviation is unknown and the sample size is small.

In this study, a teacher claims that the **average marks** of a class are **70**. A sample of five students is selected to test this claim.

---

## 2. When to Use a t-Test

A t-test is appropriate under the following conditions:

1. **Population Standard Deviation Is Unknown**  
2. **Small Sample Size (n < 30)**  
3. **Approximately Normal Data**  
4. **Comparison of Means**  
5. **Numerical (Quantitative) Data**

---

## 3. Types of t-Tests

| Type | Purpose | Example |
|------|--------|---------|
| One-sample t-test | Compare sample mean with known value | Class average vs 70 |
| Independent t-test | Compare two groups | Boys vs Girls marks |
| Paired t-test | Compare before-after results | Test scores before & after training |

---

## 4. Given Data

Sample marks:  
65, 68, 75, 80, 72  

Sample size:  
n = 5  

Claimed population mean:  
μ₀ = 70  

Significance level:  
α = 0.05  

---

## 5. Sample Mean

x̄ = (65 + 68 + 75 + 80 + 72) / 5  
x̄ = 360 / 5 = 72  

---

## 6. Sample Standard Deviation

| x | x − 72 | (x − 72)² |
|---|--------|-----------|
| 65 | −7 | 49 |
| 68 | −4 | 16 |
| 75 | 3 | 9 |
| 80 | 8 | 64 |
| 72 | 0 | 0 |

Sum of squares = 138  

s² = 138 / 4 = 34.5  
s = √34.5 ≈ 5.87  

---

## 7. Test Statistic

t = (x̄ − μ₀) / (s / √n)  
t = (72 − 70) / (5.87 / √5) ≈ 0.76  

Degrees of freedom:  
df = n − 1 = 4  

---

## 8. p-Value and Decision Rule

The **p-value** is the probability of obtaining the observed result if the null hypothesis is true.

Decision rule:

- If p ≤ 0.05 → Reject H₀  
- If p > 0.05 → Do not reject H₀  

For t = 0.76, df = 4:

| Test | p-value |
|------|---------|
| Two-tailed | ≈ 0.49 |
| One-tailed | ≈ 0.245 |

---

## 9. Hypothesis Testing Cases

### Example 1: Two-Tailed Test

H₀: μ = 70  
H₁: μ ≠ 70  

p ≈ 0.49 > 0.05  

**Decision:** Do not reject H₀  

**Conclusion:**  
There is no significant difference between the sample mean and 70.

---

### Example 2: Left-Tailed Test (Negative t)

H₁: μ < 70  

Assume:  
t = −3.0, p ≈ 0.02  

p < 0.05  

**Decision:** Reject H₀  

**Conclusion:**  
The average marks are significantly lower than 70.

---

### Example 3: Left-Tailed Test (Positive t)

Assume:  
t = 1.5, p ≈ 0.11  

p > 0.05  

**Decision:** Do not reject H₀  

**Conclusion:**  
There is no evidence that the average is less than 70.

---

### Example 4: Right-Tailed Test (Negative t)

H₁: μ > 70  

Assume:  
t = −1.2, p ≈ 0.15  

p > 0.05  

**Decision:** Do not reject H₀  

**Conclusion:**  
The average is not significantly greater than 70.

---

### Example 5: Right-Tailed Test (Positive t)

Assume:  
t = 3.1, p ≈ 0.01  

p < 0.05  

**Decision:** Reject H₀  

**Conclusion:**  
The average marks are significantly higher than 70.

---

## 10. Final Conclusion for the Given Data

For the actual sample:

t = 0.76  

| Test | p-value | Decision |
|------|---------|----------|
| Two-tailed | 0.49 | Do not reject |
| Left-tailed | 0.245 | Do not reject |
| Right-tailed | 0.245 | Do not reject |

**Overall Conclusion:**  
There is insufficient statistical evidence to reject the teacher’s claim that the class average is 70.

---

## 11. Summary of Steps

1. State hypotheses  
2. Calculate sample mean  
3. Compute standard deviation  
4. Calculate t-statistic  
5. Find p-value  
6. Compare with α  
7. Make decision  
8. Write conclusion  
