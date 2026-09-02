# 🐚 Bash — Arrays

```bash
#!/bin/bash

names=("Yuvraj" "Roman" "John")

echo ${names[0]}
echo ${names[1]}
echo ${names[2]}
```

### 🔹 Simple Explanation

- `names=(...)` → Creates an array and stores multiple names.
- `${names[0]}` → Gets the **first name**.
- `${names[1]}` → Gets the **second name**.
- `${names[2]}` → Gets the **third name**.
- Bash arrays start from **index `0`**.

### 🖥️ Output

```text
Yuvraj
Roman
John
```

### 💡 Key Idea

```text
names
  ↓
[0] Yuvraj
[1] Roman
[2] John
```

> 🚀 Arrays allow Bash scripts to **store multiple values inside one variable**.
