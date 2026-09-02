# 🐚 Bash — If / Else

```bash
#!/bin/bash

age=$1

if [ $age -ge 18 ]
then
    echo "You are an adult"
else
    echo "You are not an adult"
fi
```

### 🔹 Simple Explanation

- `age=$1` → Takes the first argument and stores it in `age`.
- `if` → Checks a condition.
- `[ $age -ge 18 ]` → Checks if age is **greater than or equal to 18**.
- `then` → Runs the code if the condition is true.
- `else` → Runs the code if the condition is false.
- `fi` → Ends the `if` statement.

### 🖥️ Run

```bash
./script.sh 20
```

### 🖥️ Output

```text
You are an adult
```

### 💡 Key Idea

```text
       Condition
           ↓
    ┌── age >= 18? ──┐
    ↓                ↓
  TRUE             FALSE
    ↓                ↓
 Adult        Not an adult
```

> 🚀 `if / else` lets a Bash script **make decisions based on conditions**.
