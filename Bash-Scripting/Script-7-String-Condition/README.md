# 🐚 Bash — String Conditions

```bash
#!/bin/bash

name=$1

if [ "$name" = "Yuvi" ]
then
    echo "Hello Yuvi"
else
    echo "Hello $name"
fi
```

### 🔹 Simple Explanation

- `=` → Checks if two strings are equal.
- `!=` → Checks if two strings are different.
- `-z` → Checks if a string is empty.
- `-n` → Checks if a string is not empty.
- `"$name"` → Gets the value stored in the `name` variable.

### 🖥️ Run

```bash
./script.sh Yuvi
```

### 🖥️ Output

```text
Hello Yuvi
```

### 💡 Key Idea

```text
$name
  ↓
"Yuvi"?
  ↓
YES → Hello Yuvi
NO  → Hello <name>
```

> 🚀 String conditions are used to **compare and check text values** in Bash.
