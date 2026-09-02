# 🐚 Bash — Variables

```bash
#!/bin/bash

name="Yuvi"

echo "Hi $name"
echo "You are looking good $name"
```

### 🔹 Simple Explanation

- `name="Yuvi"` → Creates a variable called `name` and stores `"Yuvi"` in it.
- `$name` → Gets the value stored inside the `name` variable.
- `echo "Hi $name"` → Prints `Hi Yuvi`.
- `echo "You are looking good $name"` → Prints `You are looking good Yuvi`.

### 🖥️ Output

```text
Hi Yuvi
You are looking good Yuvi
```

### 💡 Key Idea

```text
name="Yuvi"
    ↓
 $name
    ↓
  Yuvi
```

> 🚀 In Bash, **variables store values**, and `$variable_name` is used to access those values.
