# 🐚 Bash — Comparison Operators

```bash
#!/bin/bash

age=$1

if [ $age -ge 18 ]
then
    echo "You are 18 or older"
else
    echo "You are under 18"
fi
```

### 🔹 Common Comparison Operators

- `-eq` → Equal to
- `-ne` → Not equal to
- `-gt` → Greater than
- `-lt` → Less than
- `-ge` → Greater than or equal to
- `-le` → Less than or equal to

### 🖥️ Example

```bash
./script.sh 20
```

```text
You are 18 or older
```

### 💡 Key Idea

```text
20 -ge 18
     ↓
   TRUE
     ↓
Run "then"
```

> 🚀 These operators are mainly used to **compare numbers inside `if` conditions**.
