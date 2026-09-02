# 🐚 Bash — Logical Operators

```bash
#!/bin/bash

age=$1

if [ $age -ge 18 ] && [ $age -le 60 ]
then
    echo "You can work"
else
    echo "You cannot work"
fi
```

### 🔹 Simple Explanation

- `&&` → **AND** — both conditions must be true.
- `||` → **OR** — at least one condition must be true.
- `!` → **NOT** — reverses the condition.

### 🖥️ Example

```bash
./script.sh 25
```

```text
You can work
```

### 💡 Key Idea

```text
Condition 1  &&  Condition 2
     ↓              ↓
   TRUE            TRUE
          ↓
        TRUE
```

> 🚀 Logical operators let you **combine multiple conditions** in Bash.
