# 🐚 Bash — Arithmetic

```bash
#!/bin/bash

a=10
b=5

sum=$((a + b))

echo "Sum = $sum"
```

### 🔹 Simple Explanation

- `a=10` → Stores `10` in variable `a`.
- `b=5` → Stores `5` in variable `b`.
- `$((a + b))` → Performs the calculation.
- `sum=` → Stores the result in `sum`.
- `echo` → Prints the result.

### 🔢 Common Operators

- `+` → Addition
- `-` → Subtraction
- `*` → Multiplication
- `/` → Division
- `%` → Remainder

### 🖥️ Output

```text
Sum = 15
```

### 💡 Key Idea

```text
a = 10
b = 5
   ↓
$((a + b))
   ↓
  15
```

> 🚀 `$(( ))` is used to **perform arithmetic calculations in Bash**.
