# One-Sample t-Test: Complete Explanation with Applications

## 1. Introduction

A **t-test** is a statistical method used to determine whether the mean of a sample is significantly different from a claimed population mean when the population standard deviation is unknown and the sample size is small.

In this study, a teacher claims that the **average marks** of a class are **70**. A sample of five students is selected to test this claim. The purpose of the test is to check whether the sample data provides enough statistical evidence to support or reject the teacher’s claim.

---

## 2. When to Use a t-Test

A t-test is appropriate under the following conditions:

1. **Population Standard Deviation Is Unknown**  
   The true population standard deviation is usually not available, so the sample standard deviation is used.

2. **Small Sample Size (n < 30)**  
   The t-distribution is more suitable than the normal distribution for small samples.

3. **Approximately Normal Data**  
   The data should come from a population that is roughly normally distributed.

4. **Comparison of Means**  
   The t-test is used when comparing averages.

5. **Numerical (Quantitative) Data**  
   The data must be numerical, such as marks or scores.

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

The sample mean (72) is slightly higher than the claimed mean (70).  
However, this difference alone is not enough to draw a conclusion.  
We must check whether this difference is **statistically significant**.

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

The standard deviation (5.87) shows that the marks vary moderately around the mean.

---

## 7. Test Statistic

t = (x̄ − μ₀) / (s / √n)  
t = (72 − 70) / (5.87 / √5) ≈ 0.76  

Degrees of freedom:  
df = n − 1 = 4  

The t-value of **0.76** means that the sample mean is **0.76 standard errors above** the claimed mean.  
This is a small difference, suggesting weak evidence against the teacher’s claim.

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

Since all p-values are **greater than 0.05**, the evidence is **not strong enough** to reject the null hypothesis.

---

## 9. Hypothesis Testing Cases (Detailed Explanation)

---

### Example 1: Two-Tailed Test  
**Question:** *Is the average different from 70?*

H₀: μ = 70  
H₁: μ ≠ 70  

p ≈ 0.49 > 0.05  

**Decision:** Do not reject H₀  

**Explanation:**  
A two-tailed test checks for **any difference**, whether higher or lower.  
The p-value (0.49) is very large, which means the observed difference (72 vs 70) could easily happen by chance.

**Conclusion:**  
There is no significant difference between the sample mean and 70.

---

### Example 2: Left-Tailed Test (Negative t)  
**Question:** *Is the average lower than 70?*

H₁: μ < 70  

Assume:  
t = −3.0, p ≈ 0.02  

p < 0.05  

**Decision:** Reject H₀  

**Explanation:**  
A negative t-value means the sample mean is much **lower** than 70.  
The small p-value (0.02) shows that this result is unlikely due to chance.

**Conclusion:**  
The average marks are significantly lower than 70.

---

### Example 3: Left-Tailed Test (Positive t)  
**Question:** *Is the average lower than 70?*

Assume:  
t = 1.5, p ≈ 0.11  

p > 0.05  

**Decision:** Do not reject H₀  

**Explanation:**  
The sample mean is actually **higher** than 70.  
So there is no evidence to support the claim that the average is lower.

**Conclusion:**  
There is no evidence that the average is less than 70.

---

### Example 4: Right-Tailed Test (Negative t)  
**Question:** *Is the average higher than 70?*

H₁: μ > 70  

Assume:  
t = −1.2, p ≈ 0.15  

p > 0.05  

**Decision:** Do not reject H₀  

**Explanation:**  
A negative t-value means the sample mean is below 70.  
So it does not support the claim that the average is higher.

**Conclusion:**  
The average is not significantly greater than 70.

---

### Example 5: Right-Tailed Test (Positive t)  
**Question:** *Is the average higher than 70?*

Assume:  
t = 3.1, p ≈ 0.01  

p < 0.05  

**Decision:** Reject H₀  

**Explanation:**  
A large positive t-value means the sample mean is much higher than 70.  
The small p-value shows strong statistical evidence.

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

This means the observed difference between the sample mean (72) and the claimed mean (70) is **not statistically significant**.

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
