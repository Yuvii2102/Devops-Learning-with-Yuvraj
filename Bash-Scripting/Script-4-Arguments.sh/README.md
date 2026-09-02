# 🐚 Bash — Arguments

```bash
#!/bin/bash

name=$1
food=$2

echo "Hi $name"
echo "You like $food"
```

### 🔹 Simple Explanation

- `name=$1` → Stores the **first argument** in `name`.
- `food=$2` → Stores the **second argument** in `food`.
- `$1` → First argument.
- `$2` → Second argument.
- `echo "Hi $name"` → Prints the name.
- `echo "You like $food"` → Prints the food.

### 🖥️ Run the Script

```bash
./script.sh Yuvi Pizza
```

### 🖥️ Output

```text
Hi Yuvi
You like Pizza
```

### 💡 Key Idea

```text
./script.sh Yuvi Pizza
          ↓     ↓
         $1    $2
          ↓     ↓
        name  food
```

> 🚀 Bash arguments allow you to **pass values to a script when running it**.
