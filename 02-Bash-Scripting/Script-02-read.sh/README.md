# 🐚 Bash — Taking User Input

```bash
#!/bin/bash

echo "Enter your name? "
read name
echo "Hi $name"
```

### 🔹 Simple Explanation

- `#!/bin/bash` → Tells Linux to run the script using Bash.
- `echo "Enter your name?"` → Displays a message asking for your name.
- `read name` → Takes the user's input and stores it in the variable `name`.
- `echo "Hi $name"` → Prints the stored name.

### 🖥️ Example

```text
Enter your name?
Yuvi
Hi Yuvi
```

### 💡 Key Idea

```text
User Input
    ↓
read name
    ↓
$name
    ↓
Output
```

> 🚀 `read` is used to **take input from the user**, while `$name` is used to **access the stored value**.
