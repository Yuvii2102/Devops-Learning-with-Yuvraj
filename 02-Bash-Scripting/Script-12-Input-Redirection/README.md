# 🐚 Bash — Input Redirection

```bash
#!/bin/bash

echo "Enter your name:"
read name < names.txt

echo "Hi $name"
```

### 🔹 Simple Explanation

- `<` → Takes **input from a file** instead of the keyboard.
- `read name` → Reads the input and stores it in `name`.
- `names.txt` → Provides the input to the script.
- `echo` → Prints the stored value.

### 🖥️ Example

```text
names.txt
Yuvraj
```

```text
Hi Yuvraj
```

### 💡 Key Idea

```text
names.txt
    ↓
   < 
    ↓
read name
    ↓
$name
    ↓
Output
```

> 🚀 Input redirection `<` allows a command or script to **take input from a file**.
