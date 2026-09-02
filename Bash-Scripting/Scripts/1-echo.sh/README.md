<div align="center">

# Bash Scripting — Your First Shell Script

### 🐧 Understanding `#!/bin/bash` • `echo` • `sleep` • Script Execution

![Bash](https://img.shields.io/badge/Bash-Scripting-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Shell-FCC624?style=for-the-badge&logo=linux&logoColor=black)

**Write → Execute → Automate 🚀**

</div>

---

## 📌 What This Script Does

This is a simple **Bash script** that prints a conversation-like message to the terminal.

Between every message, the `sleep 3` command pauses the script for **3 seconds**.

```text
Hi Mom
   ↓
Wait 3 seconds
   ↓
Hello Yuvi
   ↓
Wait 3 seconds
   ↓
How are you?
   ↓
Wait 3 seconds
   ↓
I am fine
   ↓
Wait 3 seconds
   ↓
Script Ends
```

---

# 💻 Bash Script

```bash
#!/bin/bash

echo "Hi Mom"

sleep 3

echo "Hello Yuvi"

sleep 3

echo "How are you?"

sleep 3

echo "I am fine"

sleep 3
```

---

# 🧩 Understanding Each Command

## 1️⃣ `#!/bin/bash`

```bash
#!/bin/bash
```

This is called a **Shebang**.

It tells Linux:

> 🐧 Execute this script using the **Bash shell**.

```text
Script
  │
  ▼
#!/bin/bash
  │
  ▼
Bash Shell
  │
  ▼
Execute Commands
```

---

## 2️⃣ `echo`

```bash
echo "Hi Mom"
```

`echo` is used to **print text to the terminal**.

### Example

```bash
echo "Hello Yuvi"
```

### Output

```text
Hello Yuvi
```

---

## 3️⃣ `sleep`

```bash
sleep 3
```

`sleep` pauses the execution of the script.

The number `3` means:

```text
3 seconds
```

For example:

```bash
echo "Hello"
sleep 3
echo "World"
```

The output will be:

```text
Hello
```

⏳ **3 seconds later:**

```text
World
```

---

# 🗺️ Simple Execution Diagram

```text
                 🚀 Bash Script
                       │
                       ▼
                ┌──────────────┐
                │ #!/bin/bash  │
                └──────┬───────┘
                       │
                       ▼
              ┌─────────────────┐
              │ echo "Hi Mom"   │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    sleep 3      │
              │   ⏳ 3 seconds  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ echo "Hello     │
              │      Yuvi"      │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    sleep 3      │
              │   ⏳ 3 seconds  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ echo "How are   │
              │      you?"      │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    sleep 3      │
              │   ⏳ 3 seconds  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ echo "I am fine"│
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    sleep 3      │
              │   ⏳ 3 seconds  │
              └────────┬────────┘
                       │
                       ▼
                    🏁 END
```

---

# 🖥️ Expected Terminal Output

When you execute the script:

```bash
./script.sh
```

You will first see:

```text
Hi Mom
```

⏳ After 3 seconds:

```text
Hello Yuvi
```

⏳ After another 3 seconds:

```text
How are you?
```

⏳ After another 3 seconds:

```text
I am fine
```

⏳ After the final 3-second delay:

```text
🏁 Script Ends
```

---

# 🚀 How to Run the Script

## 1️⃣ Create the Script

Create a file named:

```bash
script.sh
```

You can create it using:

```bash
touch script.sh
```

---

## 2️⃣ Add the Bash Code

Open the file:

```bash
vim script.sh
```

Or:

```bash
nano script.sh
```

Add:

```bash
#!/bin/bash

echo "Hi Mom"

sleep 3

echo "Hello Yuvi"

sleep 3

echo "How are you?"

sleep 3

echo "I am fine"

sleep 3
```

---

## 3️⃣ Give Execute Permission

```bash
chmod +x script.sh
```

### Why?

Linux needs execute permission before you can directly run the script using:

```bash
./script.sh
```

---

## 4️⃣ Execute the Script

```bash
./script.sh
```

### Execution Flow

```text
script.sh
    │
    ▼
chmod +x
    │
    ▼
./script.sh
    │
    ▼
Bash executes the script
    │
    ▼
echo + sleep
    │
    ▼
🏁 Script completes
```

---

# ⚡ Another Way to Run It

You don't always need to make the script executable.

You can directly tell Bash to execute it:

```bash
bash script.sh
```

### Difference

| Method | Requires `chmod +x`? | How it works |
|---|:---:|---|
| `./script.sh` | ✅ Yes | Linux executes the file directly |
| `bash script.sh` | ❌ No | Bash explicitly executes the file |

---

# 🧠 Important Concepts Learned

| Command | Meaning |
|---|---|
| `#!/bin/bash` | Use Bash to execute the script |
| `echo` | Print text |
| `sleep` | Pause execution |
| `chmod +x` | Give execute permission |
| `./script.sh` | Execute the script |
| `bash script.sh` | Run script using Bash |

---

# 🔥 What I Learned

- 🐧 **Shebang** tells Linux which interpreter to use.
- 🖨️ **`echo`** prints information to the terminal.
- ⏳ **`sleep`** pauses script execution.
- 🔐 **`chmod +x`** gives execute permission.
- 🚀 **`./script.sh`** executes an executable script.
- 🐚 **`bash script.sh`** runs the script explicitly through Bash.
- 🔄 Bash executes commands **from top to bottom**.
- 🤖 Bash scripts can later be used to automate DevOps tasks.

---

# 🚀 From Simple Script to DevOps Automation

This simple script is the beginning of **shell automation**.

Today:

```bash
echo "Hi Mom"
sleep 3
echo "Hello Yuvi"
```

Later, Bash can automate DevOps tasks:

```bash
#!/bin/bash

git pull

docker build -t my-app .

docker push my-app

kubectl apply -f deployment.yaml

echo "🚀 Deployment completed!"
```

### DevOps Automation Flow

```mermaid
flowchart LR
    A["🐚 Bash Script"] --> B["🔀 Git"]
    B --> C["🐳 Docker"]
    C --> D["☸️ Kubernetes"]
    D --> E["🚀 Deployment"]
    E --> F["📊 Monitoring"]
```

---

<div align="center">

## 🐚 Bash Scripting

### Start Small → Automate Everything

**Linux → Bash → Git → Docker → Kubernetes → DevOps 🚀**

# 🏁 BASH SCRIPTING — DAY 01 COMPLETE

</div>
