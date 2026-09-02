# 🐚 Bash — Pipes

```bash
#!/bin/bash

echo "Yuvraj Roman John" | tr ' ' '\n'
```

### 🔹 Simple Explanation

- `|` → Sends the **output of one command** to another command.
- `echo` → Produces the names.
- `tr ' ' '\n'` → Replaces spaces with new lines.
- The second command receives the output from the first command.

### 🖥️ Output

```text
Yuvraj
Roman
John
```

### 💡 Key Idea

```text
Command 1
   ↓
   |
   ↓
Command 2
   ↓
Output
```

> 🚀 Pipes `|` are used to **connect commands together** and pass output from one command to another.
