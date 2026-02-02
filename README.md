# assignment

---

## 1. What is a function (conceptually)?

A **function** is:

* a **named block of reusable code**
* that **takes input** (optional),
* **does some work**,
* and **returns output** (optional).

Think of it as a **machine**:

```
input  →  function  →  output
```

Why functions matter:

* Avoid repeating code
* Make programs readable
* Break big problems into small logical parts
* Essential for real-world Python (data science, ML, backend, automation)

---

## 2. Basic syntax of a function

```python
def function_name():
    # code inside function
```

Example:

```python
def greet():
    print("Hello, welcome to Python!")
```

Calling the function:

```python
greet()
```

📌 **Important**

* `def` = define
* Indentation **matters**
* Nothing runs until the function is **called**

---

## 3. Functions with parameters (inputs)

### Example 1: One parameter

```python
def greet(name):
    print("Hello", name)
```

Call it:

```python
greet("Amit")
greet("Riya")
```

Output:

```
Hello Amit
Hello Riya
```

Here:

* `name` is a **parameter**
* `"Amit"` is an **argument**

---

### Example 2: Multiple parameters

```python
def add(a, b):
    print(a + b)
```

```python
add(10, 20)
add(5, 7)
```

---

## 4. `return` vs `print` (VERY IMPORTANT)

### ❌ Using `print` only

```python
def add(a, b):
    print(a + b)
```

Problem: you **cannot reuse** the result.

---

### ✅ Using `return`

```python
def add(a, b):
    return a + b
```

```python
result = add(10, 20)
print(result)
```

📌 **Rule**

* `print()` → shows output
* `return` → sends value back to program

Most real programs **use return**, not print.

---

## 5. Function with logic (if–else)

```python
def check_even_odd(number):
    if number % 2 == 0:
        return "Even"
    else:
        return "Odd"
```

```python
check_even_odd(10)
check_even_odd(7)
```

---

## 6. Default parameters

```python
def greet(name="Student"):
    print("Hello", name)
```

```python
greet()
greet("Rahul")
```

Output:

```
Hello Student
Hello Rahul
```

---

## 7. Function returning multiple values

```python
def calculate(a, b):
    sum_ = a + b
    diff = a - b
    return sum_, diff
```

```python
x, y = calculate(10, 5)
print(x)
print(y)
```

Python returns a **tuple** internally.

---

## 8. Functions with lists

```python
def total_marks(marks):
    return sum(marks)
```

```python
marks = [80, 75, 90]
total_marks(marks)
```

---

## 9. Common beginner mistakes 🚨

### ❌ Forgetting to call the function

```python
def greet():
    print("Hi")

# greet not called
```

### ❌ Using `print` instead of `return`

```python
x = add(10, 20)  # x becomes None if add uses print
```

### ❌ Wrong indentation

```python
def greet():
print("Hi")   # ERROR
```

---

## 10. Practice (VERY IMPORTANT)

Try these **without looking at solutions**:

1. Write a function `square(n)` that returns square of a number
2. Write a function `is_positive(n)` → returns `"Positive"` or `"Negative"`
3. Write a function `average(numbers)` → takes a list and returns average
4. Write a function `count_vowels(word)`

---

## 11. When should YOU use functions?

Use a function when:

* Code repeats more than once
* Logic can be named (e.g., `calculate_tax`)
* You want cleaner, professional code

---

## 12. What we’ll do next (recommended order)

If you say **yes**, I’ll teach next:

1. Function + loops (real logic)
2. `*args` and `**kwargs`
3. Lambda functions
4. Real business-style examples (marks, salary, GST, data analysis)
5. How functions are used in **Pandas & ML**

👉 Tell me:
**Do you want more practice questions or move to advanced functions?**


