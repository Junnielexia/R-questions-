# R project

```
# 🧠 Let's go step by step! 🐣🐾

---

## 🧰 First, What Are These R Tools?

---

### ✅ `c()` — Combine (📦)

Use `c()` to combine numbers into a list.

```r
c(1, 2, 3)
# Output: [1] 1 2 3
```

Think of it like putting numbers in a box. 📦

---

### ✅ a:b — Count from a to b (🖐️)

```r
1:5
# Output: [1] 1 2 3 4 5
```

It just counts up from the first number to the second one.

---

### ✅ `seq()` — Sequence Robot (🤖)

This function creates sequences with different rules!

#### 🔹 Count normally:
```r
seq(1, 5)
# Output: [1] 1 2 3 4 5
```

#### 🔹 Skip numbers (use `by =`):
```r
seq(1, 9, by = 2)
# Output: [1] 1 3 5 7 9
```

#### 🔹 Spread evenly (use `length.out`) 📏:
```r
seq(0, 15, length.out = 4)
# Output: [1]  0  5 10 15
```

---

## 🧪 Questions and Solutions

---

### ✅ Question 1
Create the vector `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]` in three ways: once using `c()`, once using `a:b`, and once using `seq()`.

#### 📦 Using `c()`:
```r
v1a <- c(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
```

#### 🔢 Using `:`:
```r
v1b <- 1:10
```

#### 🤖 Using `seq()`:
```r
v1c <- seq(1, 10)
```

---

### ✅ Question 2
Create the vector `[2.1, 4.1, 6.1, 8.1]` in two ways, once using `c()` and once using `seq()`

#### 📦 Using `c()`:
```r
v2a <- c(2.1, 4.1, 6.1, 8.1)
```

#### 🤖 Using `seq()`:
```r
v2b <- seq(2.1, 8.1, by = 2)
```

---

### ✅ Question 3
Create the vector `[0, 5, 10, 15]` in 3 ways: using `c()`, `seq()` with a `by` argument, and `seq()` with a `length.out` argument.

#### 📦 Using `c()`:
```r
v3a <- c(0, 5, 10, 15)
```

#### 🪜 Using `seq()` with `by`:
```r
v3b <- seq(0, 15, by = 5)
```

#### 📏 Using `seq()` with `length.out`:
```r
v3c <- seq(0, 15, length.out = 4)
```

---

### ✅ Question 4
Create the vector `[101, 102, 103, 200, 205, 210, 1000, 1100, 1200]` using a combination of the `c()` and `seq()` functions

```r
v4 <- c(seq(101, 103), seq(200, 210, 5), seq(1000, 1200, 100))
```

**Breakdown:**
- `seq(101, 103)` → `[101, 102, 103]`
- `seq(200, 210, 5)` → `[200, 205, 210]`
- `seq(1000, 1200, 100)` → `[1000, 1100, 1200]`
- `c(...)` combines them all into one vector.

---

### ✅ Question 5
A new batch of 100 pirates are boarding your ship and need new swords. You have 10 scimitars, 40 broadswords, and 50 cutlasses that you need to distribute evenly to the 100 pirates as they board. Create a vector of length 100 where there is 1 scimitar, 4 broadswords, and 5 cutlasses in each group of 10.

```r
group <- c(rep("scimitar", 1), rep("broadsword", 4), rep("cutlass", 5))
v5 <- rep(group, 10)
```

---

### ✅ Question 6
Create a vector that repeats the integers from 1 to 5, 10 times. That is `[1, 2, 3, 4, 5, 1, 2, 3, 4, 5, ...]`. The length of the vector should be 50!

```r
v6 <- rep(1:5, 10)
```

---

### ✅ Question 7
Now, create the same vector as before, but this time repeat 1, 10 times, then 2, 10 times, etc., That is `[1, 1, 1, ..., 2, 2, 2, ..., ... 5, 5, 5]`. The length of the vector should also be 50.

```r
v7 <- rep(1:5, each = 10)
```

---

### ✅ Question 8
Create a vector containing 50 samples from a Normal distribution with a population mean of 20 and standard deviation of 2.

```r
v8 <- rnorm(50, mean = 20, sd = 2)
```

---

### ✅ Question 9
Create a vector containing 25 samples from a Uniform distribution with a lower bound of -100 and an upper bound of -50.

```r
v9 <- runif(25, min = -100, max = -50)
```

---

## 🎓 Summary

You've learned how to:
- Combine values using `c()`
- Count with `:`
- Generate sequences using `seq()`
- Repeat values using `rep()`
- Generate random values using `rnorm()` and `runif()`

These are the building blocks for working with data in R! 🧱💻
```
