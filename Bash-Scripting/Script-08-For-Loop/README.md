# 🐚 Bash — For Loop

```bash
#!/bin/bash

for name in Yuvi Roman John
do
    echo "Hi $name"
done
```

### 🔹 Simple Explanation

- `for` → Starts the loop.
- `name` → Variable that stores each value.
- `in` → Provides the values to loop through.
- `do` → Starts the commands to repeat.
- `echo "Hi $name"` → Prints each name.
- `done` → Ends the loop.

### 🖥️ Output

```text
Hi Yuvi
Hi Roman
Hi John
```

### 💡 Key Idea

```text
Yuvi
 ↓
Roman
 ↓
John
 ↓
Repeat for each value
```

> 🚀 A `for` loop is used to **repeat a command for multiple values**.
