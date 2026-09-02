<div align="center">

# 🐧 Linux Commands for DevOps

### 📚 A Practical Linux Command Reference

![Linux](https://img.shields.io/badge/Linux-Commands-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-Shell-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![DevOps](https://img.shields.io/badge/DevOps-Essentials-0A0A0A?style=for-the-badge&logo=devdotto)

**Learn → Practice → Troubleshoot → Automate**

</div>

---

# 📚 Table of Contents

- [📍 Command Location](#-command-location)
- [📋 List Operations](#-list-operations)
- [📂 Changing Directories](#-changing-directories)
- [📁 File & Folder Operations](#-file--folder-operations)
- [📖 Viewing Files](#-viewing-files)
- [🔍 Searching Files](#-searching-files)
- [🔎 Searching Inside Files](#-searching-inside-files)
- [📖 Manual & Help](#-manual--help)
- [🖥️ System Commands](#️-system-commands)
- [⚙️ Process Management](#️-process-management)
- [👤 User Management](#-user-management)
- [🔐 Permissions](#-permissions)
- [👑 Ownership](#-ownership)
- [🌐 Networking](#-networking)
- [📥 Downloading Files](#-downloading-files)
- [📦 Compression & Archives](#-compression--archives)
- [🔤 Text Processing](#-text-processing)
- [🔗 Pipes](#-pipes)
- [🕘 Command History](#-command-history)
- [🌱 Environment Variables](#-environment-variables)
- [🧩 Aliases](#-aliases)
- [🔀 Operators](#-operators)
- [🏃 Background Jobs](#-background-jobs)
- [🔑 Base64](#-base64)
- [🚀 Practical DevOps Examples](#-practical-devops-examples)
- [⭐ Commands to Master](#-commands-to-master)

---

# 📍 Command Location

> 🔎 **Use these commands when you want to know where a Linux command/executable is located.**

- ### `which`
  **Purpose:** Find the path of an executable.

  ```bash
  which python
  ```

  **Example output:**

  ```text
  /usr/bin/python
  ```

- ### `whereis`
  **Purpose:** Find the binary, source and manual locations of a command.

  ```bash
  whereis python
  ```

  **Example:**

  ```text
  python: /usr/bin/python /usr/lib/python3
  ```

---

# 📋 List Operations

> 📂 **Use `ls` commands to inspect files, directories and permissions.**

- ### `ls`
  **Purpose:** List files and directories.

  ```bash
  ls
  ```

- ### `ls -a`
  **Purpose:** Show all files, including hidden files.

  ```bash
  ls -a
  ```

- ### `ls -l`
  **Purpose:** Show detailed information such as permissions, owner, group, size and modification time.

  ```bash
  ls -l
  ```

- ### `ls -R`
  **Purpose:** List directories recursively.

  ```bash
  ls -R
  ```

- ### `ls -la`
  **Purpose:** Show detailed information including hidden files.

  ```bash
  ls -la
  ```

  ⭐ **One of the most commonly used Linux commands in DevOps.**

---

# 📂 Changing Directories

> 🧭 **Use `cd` commands to move around the Linux filesystem.**

- ### `cd <directory>`
  **Purpose:** Change to a directory.

  ```bash
  cd project
  ```

- ### `cd ..`
  **Purpose:** Go one directory back.

  ```bash
  cd ..
  ```

- ### `cd`
  **Purpose:** Go to your home directory.

  ```bash
  cd
  ```

- ### `cd ~`
  **Purpose:** Go to your home directory.

  ```bash
  cd ~
  ```

- ### `cd -`
  **Purpose:** Return to the previous directory.

  ```bash
  cd -
  ```

- ### `cd ../<directory>`
  **Purpose:** Access a directory relative to the parent directory.

  ```bash
  cd ../project
  ```

- ### `cd <path>`
  **Purpose:** Navigate using an absolute or relative path.

  ```bash
  cd /home/ubuntu/project
  ```

---

# 📁 File & Folder Operations

> 🛠️ **These commands are used constantly for managing files and directories.**

- ### `mkdir`
  **Purpose:** Create a new directory.

  ```bash
  mkdir project
  ```

- ### `mkdir -p`
  **Purpose:** Create nested directories in one command.

  ```bash
  mkdir -p project/app/logs
  ```

  **Result:**

  ```text
  project/
  └── app/
      └── logs/
  ```

- ### `touch`
  **Purpose:** Create an empty file.

  ```bash
  touch test.txt
  ```

- ### `pwd`
  **Purpose:** Display the present working directory.

  ```bash
  pwd
  ```

- ### `cat`
  **Purpose:** Display the contents of a file.

  ```bash
  cat test.txt
  ```

- ### `cat > <filename>`
  **Purpose:** Create or overwrite a file.

  ```bash
  cat > test.txt
  ```

  Type your content and press:

  ```text
  Ctrl + D
  ```

- ### `cat >> <filename>`
  **Purpose:** Append content to a file.

  ```bash
  cat >> test.txt
  ```

- ### `echo`
  **Purpose:** Print text.

  ```bash
  echo "Hello Linux"
  ```

  **Write text to a file:**

  ```bash
  echo "Hello Linux" > test.txt
  ```

  **Append text:**

  ```bash
  echo "Learning DevOps" >> test.txt
  ```

- ### `cat <file1> <file2>`
  **Purpose:** Display multiple files.

  ```bash
  cat file1.txt file2.txt
  ```

- ### `cat <file1> <file2> > <newfile>`
  **Purpose:** Merge the contents of two files.

  ```bash
  cat file1.txt file2.txt > combined.txt
  ```

- ### `cp`
  **Purpose:** Copy a file.

  ```bash
  cp file.txt backup.txt
  ```

  **Copy to another directory:**

  ```bash
  cp file.txt /tmp/
  ```

- ### `mv`
  **Purpose:** Move a file.

  ```bash
  mv file.txt /tmp/
  ```

  **Rename a file:**

  ```bash
  mv old.txt new.txt
  ```

- ### `rm`
  **Purpose:** Remove a file.

  ```bash
  rm test.txt
  ```

- ### `rm -r`
  **Purpose:** Remove a directory and its contents.

  ```bash
  rm -r project/
  ```

- ### `rm -rf`
  **Purpose:** Forcefully remove a directory and everything inside it.

  ```bash
  rm -rf project/
  ```

  ⚠️ **Use `rm -rf` very carefully.**

---

# 📖 Viewing Files

> 👀 **These commands are especially useful when working with configuration files and application logs.**

- ### `head`
  **Purpose:** Display the first 10 lines of a file.

  ```bash
  head file.txt
  ```

- ### `head -n`
  **Purpose:** Display a specific number of lines from the beginning.

  ```bash
  head -n 5 file.txt
  ```

- ### `tail`
  **Purpose:** Display the last 10 lines.

  ```bash
  tail file.txt
  ```

- ### `tail -n`
  **Purpose:** Display a specific number of lines from the end.

  ```bash
  tail -n 5 file.txt
  ```

- ### `tail -f`
  **Purpose:** Continuously monitor a file as new content is added.

  ```bash
  tail -f application.log
  ```

  ⭐ **Extremely useful for real-time log monitoring.**

  ```bash
  tail -f /var/log/syslog
  ```

---

# 🔍 Searching Files

> 🔎 **Use `find` when you need to locate files or directories.**

- ### `find .`
  **Purpose:** Search from the current directory.

  ```bash
  find .
  ```

- ### `find . -name`
  **Purpose:** Find a specific file by name.

  ```bash
  find . -name "config.txt"
  ```

- ### `find . -type d`
  **Purpose:** Show directories only.

  ```bash
  find . -type d
  ```

- ### `find . -type f`
  **Purpose:** Show files only.

  ```bash
  find . -type f
  ```

- ### `find . -type f -name "*.txt"`
  **Purpose:** Find all `.txt` files.

  ```bash
  find . -type f -name "*.txt"
  ```

- ### `find . -type f -iname "*.txt"`
  **Purpose:** Case-insensitive filename search.

  ```bash
  find . -type f -iname "*.txt"
  ```

- ### `find . -type f -mmin -20`
  **Purpose:** Find files modified within the last 20 minutes.

  ```bash
  find . -type f -mmin -20
  ```

- ### `find . -type f -mmin +20`
  **Purpose:** Find files modified more than 20 minutes ago.

  ```bash
  find . -type f -mmin +20
  ```

- ### `find . -maxdepth 2 -type f`
  **Purpose:** Search only up to two directory levels.

  ```bash
  find . -maxdepth 2 -type f
  ```

- ### `find . -type f -size +1k`
  **Purpose:** Find files larger than 1 KB.

  ```bash
  find . -type f -size +1k
  ```

- ### `find . -type f -size +100M`
  **Purpose:** Find files larger than 100 MB.

  ```bash
  find . -type f -size +100M
  ```

- ### `locate`
  **Purpose:** Quickly search for files.

  ```bash
  locate nginx.conf
  ```

  💡 `locate` uses an indexed database, while `find` searches the filesystem directly.

---

# 🔎 Searching Inside Files

> 🕵️ **`grep` is one of the most important Linux commands for DevOps troubleshooting.**

- ### `grep`
  **Purpose:** Search for a keyword inside a file.

  ```bash
  grep "ERROR" application.log
  ```

- ### `grep -i`
  **Purpose:** Case-insensitive search.

  ```bash
  grep -i "error" application.log
  ```

- ### `grep -w`
  **Purpose:** Match a complete word.

  ```bash
  grep -w "error" application.log
  ```

- ### `grep -n`
  **Purpose:** Show matching line numbers.

  ```bash
  grep -n "ERROR" application.log
  ```

- ### `grep -B`
  **Purpose:** Show lines before a match.

  ```bash
  grep -B 2 "ERROR" application.log
  ```

- ### `grep -A`
  **Purpose:** Show lines after a match.

  ```bash
  grep -A 2 "ERROR" application.log
  ```

- ### `grep -C`
  **Purpose:** Show lines before and after a match.

  ```bash
  grep -C 2 "ERROR" application.log
  ```

- ### `grep -r`
  **Purpose:** Search recursively inside directories.

  ```bash
  grep -r "ERROR" .
  ```

- ### `grep -win`
  **Purpose:** Whole word + case-insensitive + line number.

  ```bash
  grep -win "error" ./*.txt
  ```

- ### `grep -win -r`
  **Purpose:** Recursively search using all three options.

  ```bash
  grep -win -r "error" .
  ```

---

# 📖 Manual & Help

> 📚 **When you don't know how a command works, ask Linux itself.**

- ### `man`
  **Purpose:** Open the manual page for a command.

  ```bash
  man ls
  ```

  Examples:

  ```bash
  man chmod
  man find
  man grep
  ```

- ### `--help`
  **Purpose:** Display command usage and options.

  ```bash
  ls --help
  ```

  Example:

  ```bash
  find --help
  ```

---

# 🖥️ System Commands

> 🖥️ **Use these commands to understand the server's resources and system information.**

- ### `ps aux`
  **Purpose:** Display running processes.

  ```bash
  ps aux
  ```

  **Search for a process:**

  ```bash
  ps aux | grep nginx
  ```

- ### `df -h`
  **Purpose:** Check filesystem disk usage.

  ```bash
  df -h
  ```

  `-h` = Human-readable.

- ### `du -h`
  **Purpose:** Check directory/file disk usage.

  ```bash
  du -h
  ```

- ### `du -sh`
  **Purpose:** Show the total size of a directory.

  ```bash
  du -sh /var/log
  ```

- ### `sudo`
  **Purpose:** Execute a command with administrator privileges.

  ```bash
  sudo apt update
  ```

- ### `sort`
  **Purpose:** Sort lines in a file.

  ```bash
  sort names.txt
  ```

  **Reverse order:**

  ```bash
  sort -r names.txt
  ```

- ### `uname`
  **Purpose:** Display system information.

  ```bash
  uname
  ```

- ### `uname -a`
  **Purpose:** Display complete system information.

  ```bash
  uname -a
  ```

- ### `uname -r`
  **Purpose:** Display the Linux kernel version.

  ```bash
  uname -r
  ```

- ### `lscpu`
  **Purpose:** Display CPU information.

  ```bash
  lscpu
  ```

- ### `free -h`
  **Purpose:** Display memory usage in human-readable format.

  ```bash
  free -h
  ```

- ### `vmstat`
  **Purpose:** Display virtual memory and system statistics.

  ```bash
  vmstat
  ```

- ### `lsof`
  **Purpose:** List open files and the processes using them.

  ```bash
  lsof
  ```

  **Find which process is using port `8080`:**

  ```bash
  sudo lsof -i :8080
  ```

- ### `xdg-open`
  **Purpose:** Open a file or directory using a graphical application.

  ```bash
  xdg-open .
  ```

---

# ⚙️ Process Management

> ⚡ **Processes are programs currently running on your Linux system.**

- ### `top`
  **Purpose:** Monitor running processes in real time.

  ```bash
  top
  ```

  Useful for checking:

  - CPU usage
  - Memory usage
  - Running processes
  - System load

- ### `kill`
  **Purpose:** Terminate a process using its PID.

  ```bash
  kill 1234
  ```

- ### `kill -9`
  **Purpose:** Forcefully terminate a process.

  ```bash
  kill -9 1234
  ```

  ⚠️ Prefer normal `kill` before using `kill -9`.

---

# 👤 User Management

> 👤 **Linux is a multi-user operating system, so user management is important for servers and DevOps.**

- ### `whoami`
  **Purpose:** Display the current user.

  ```bash
  whoami
  ```

- ### `useradd`
  **Purpose:** Create a new user.

  ```bash
  sudo useradd devops
  ```

- ### `passwd`
  **Purpose:** Set or change a user's password.

  ```bash
  sudo passwd devops
  ```

- ### `su`
  **Purpose:** Switch to another user.

  ```bash
  su - devops
  ```

---

# 🔐 Permissions

> 🔒 **Linux permissions control who can read, write and execute files.**

### Permission Values

```text
r = Read    = 4
w = Write   = 2
x = Execute = 1
```

### Permission Groups

```text
u = User / Owner
g = Group
o = Others
```

- ### `chmod 777`
  **Purpose:** Give read, write and execute permissions to everyone.

  ```bash
  chmod 777 file.txt
  ```

  Calculation:

  ```text
  4 + 2 + 1 = 7
  ```

  ⚠️ Avoid `777` unless specifically required.

- ### `chmod 755`
  **Purpose:** Common permission for executable scripts.

  ```bash
  chmod 755 script.sh
  ```

  Meaning:

  ```text
  Owner  → rwx → 7
  Group  → r-x → 5
  Others → r-x → 5
  ```

- ### `chmod u=rwx,g=rx,o=r`
  **Purpose:** Set permissions using symbolic notation.

  ```bash
  chmod u=rwx,g=rx,o=r file.txt
  ```

- ### `chmod +x`
  **Purpose:** Add execute permission.

  ```bash
  chmod +x script.sh
  ```

- ### `find . -perm 777`
  **Purpose:** Find files/directories with permission `777`.

  ```bash
  find . -perm 777
  ```

---

# 👑 Ownership

> 👑 **Ownership determines which user and group own a file or directory.**

- ### `chown`
  **Purpose:** Change file ownership.

  ```bash
  sudo chown root file.txt
  ```

- ### `chown user:group`
  **Purpose:** Change both owner and group.

  ```bash
  sudo chown ubuntu:ubuntu file.txt
  ```

- ### `chown -R`
  **Purpose:** Change ownership recursively.

  ```bash
  sudo chown -R ubuntu:ubuntu project/
  ```

  ⭐ Common DevOps example:

  ```bash
  sudo chown -R ubuntu:ubuntu /var/www/app
  ```

---

# 🌐 Networking

> 🌍 **These commands help troubleshoot connectivity, DNS and ports.**

- ### `ping`
  **Purpose:** Test network connectivity.

  ```bash
  ping google.com
  ```

  Send only 4 packets:

  ```bash
  ping -c 4 google.com
  ```

- ### `nslookup`
  **Purpose:** Check DNS resolution.

  ```bash
  nslookup google.com
  ```

- ### `hostname`
  **Purpose:** Display the system hostname.

  ```bash
  hostname
  ```

- ### `netstat`
  **Purpose:** Display network connections.

  ```bash
  netstat
  ```

  Show listening ports:

  ```bash
  netstat -tulnp
  ```

- ### `ss`
  **Purpose:** Modern tool for checking sockets and listening ports.

  ```bash
  ss -tulnp
  ```

  Check a specific port:

  ```bash
  ss -tulnp | grep 8080
  ```

---

# 📥 Downloading Files

> 📦 **Download files directly from the terminal.**

- ### `wget`
  **Purpose:** Download a file from a URL.

  ```bash
  wget https://example.com/file.zip
  ```

  Example:

  ```bash
  wget https://example.com/app.tar.gz
  ```

---

# 📦 Compression & Archives

> 🗜️ **Useful for backups, deployments and transferring files.**

- ### `zip`
  **Purpose:** Create a ZIP archive.

  ```bash
  zip backup.zip file1.txt file2.txt
  ```

- ### `zip -r`
  **Purpose:** Zip an entire directory recursively.

  ```bash
  zip -r backup.zip project/
  ```

- ### `unzip`
  **Purpose:** Extract a ZIP archive.

  ```bash
  unzip backup.zip
  ```

---

# 🔤 Text Processing

> 🔤 **Linux provides powerful tools for manipulating and processing text.**

- ### `echo`
  **Purpose:** Print text.

  ```bash
  echo "Hello DevOps"
  ```

- ### `sort`
  **Purpose:** Sort lines.

  ```bash
  sort names.txt
  ```

- ### `cut`
  **Purpose:** Extract characters from a file.

  ```bash
  cut -c 1-5 file.txt
  ```

- ### `cut -d -f`
  **Purpose:** Extract a specific column.

  ```bash
  cut -d "," -f 1 users.csv
  ```

  Meaning:

  ```text
  -d "," → comma is the delimiter
  -f 1   → extract column 1
  ```

- ### `tr`
  **Purpose:** Translate or replace characters.

  Convert lowercase to uppercase:

  ```bash
  echo "hello" | tr 'a-z' 'A-Z'
  ```

  Output:

  ```text
  HELLO
  ```

- ### `diff`
  **Purpose:** Compare two files.

  ```bash
  diff file1.txt file2.txt
  ```

  ⭐ DevOps example:

  ```bash
  diff config-dev.yaml config-prod.yaml
  ```

---

# 🔗 Pipes

> 🔗 **A pipe `|` sends the output of one command into another command.**

### Basic Syntax

```bash
command1 | command2
```

- ### Example 1 — Search History

  ```bash
  history | grep kubectl
  ```

- ### Example 2 — Search Processes

  ```bash
  ps aux | grep nginx
  ```

- ### Example 3 — Kubernetes

  ```bash
  kubectl get pods | grep api
  ```

### Flow

```text
Command 1
    │
    │ Output
    ▼
   Pipe
    │
    ▼
Command 2
```

⭐ Pipes are extremely important for Linux troubleshooting and shell scripting.

---

# 🕘 Command History

> 🕘 **Use history to find and reuse commands you've already executed.**

- ### `history`
  **Purpose:** Display command history.

  ```bash
  history
  ```

- ### `history | grep`
  **Purpose:** Search command history.

  ```bash
  history | grep kubectl
  ```

- ### `!<number>`
  **Purpose:** Execute a command using its history number.

  ```bash
  !125
  ```

- ### `!!`
  **Purpose:** Execute the previous command.

  ```bash
  !!
  ```

  Example:

  ```bash
  sudo !!
  ```

---

# 🌱 Environment Variables

> 🌱 **Environment variables store configuration values used by the shell and applications.**

- ### `printenv`
  **Purpose:** Display environment variables.

  ```bash
  printenv
  ```

- ### `echo $PATH`
  **Purpose:** Display the PATH variable.

  ```bash
  echo $PATH
  ```

- ### `echo $HOME`
  **Purpose:** Display the user's home directory.

  ```bash
  echo $HOME
  ```

- ### `echo $USER`
  **Purpose:** Display the current username.

  ```bash
  echo $USER
  ```

- ### `export`
  **Purpose:** Create/set an environment variable.

  ```bash
  export APP_ENV=production
  ```

  Check it:

  ```bash
  echo $APP_ENV
  ```

---

# 🧩 Aliases

> ⚡ **Aliases create shortcuts for frequently used commands.**

- ### Edit `.bashrc`

  ```bash
  vi ~/.bashrc
  ```

- ### Create an alias

  ```bash
  alias ll='ls -la'
  ```

- ### Reload `.bashrc`

  ```bash
  source ~/.bashrc
  ```

- ### Use the alias

  ```bash
  ll
  ```

### ⭐ Kubernetes Alias

```bash
alias k='kubectl'
```

Reload:

```bash
source ~/.bashrc
```

Now you can use:

```bash
k get pods
```

Instead of:

```bash
kubectl get pods
```

---

# 🔀 Operators

> 🔀 **Operators allow you to control how multiple commands execute.**

- ### `;` — Sequential execution

  **Purpose:** Run commands one after another.

  ```bash
  echo "Hello"; echo "World"
  ```

- ### `&&` — Run if successful

  **Purpose:** Run the second command only if the first succeeds.

  ```bash
  mkdir project && cd project
  ```

- ### `||` — Run if failed

  **Purpose:** Run the second command if the first command fails.

  ```bash
  mkdir project || echo "Directory creation failed"
  ```

- ### `&` — Background execution

  **Purpose:** Run a command in the background.

  ```bash
  ping google.com &
  ```

### ⭐ Combined Example

```bash
mkdir project && cd project
```

Flow:

```text
mkdir project
      │
      ▼
  Successful?
    /     \
  YES      NO
   │        │
   ▼        ▼
  cd      STOP
project
```

---

# 🏃 Background Jobs

> 🏃 **Run long-running commands without blocking the terminal.**

- ### Run in background

  ```bash
  sleep 100 &
  ```

- ### `jobs`
  **Purpose:** Show background jobs.

  ```bash
  jobs
  ```

- ### `Ctrl + Z`
  **Purpose:** Suspend the current foreground process.

  ```text
  Ctrl + Z
  ```

- ### `bg`
  **Purpose:** Continue a suspended process in the background.

  ```bash
  bg
  ```

- ### `fg`
  **Purpose:** Bring a background job to the foreground.

  ```bash
  fg
  ```

---

# 🔑 Base64

> 🔐 **Base64 converts data into a text representation. It is NOT encryption.**

- ### Encode

  ```bash
  echo -n 'username' | base64
  ```

  Example output:

  ```text
  dXNlcm5hbWU=
  ```

- ### Decode

  ```bash
  echo 'dXNlcm5hbWU=' | base64 -d
  ```

  Output:

  ```text
  username
  ```

### ⚠️ Important

> **Base64 = Encoding, NOT Encryption.**

This is especially important when working with **Kubernetes Secrets**.

---

# 🚀 Practical DevOps Examples

## 🔍 1. Find where you are

```bash
pwd
```

## 📋 2. List everything

```bash
ls -la
```

## 📂 3. Navigate to logs

```bash
cd /var/log
```

## 📜 4. Monitor application logs

```bash
tail -f application.log
```

## 🔎 5. Search logs for errors

```bash
grep -i "error" application.log
```

## 🔎 6. Search logs recursively

```bash
grep -ri "error" /var/log/
```

## ⚙️ 7. Check a running application

```bash
ps aux | grep nginx
```

## 🌐 8. Check listening ports

```bash
ss -tulnp
```

## 🔌 9. Check a specific port

```bash
ss -tulnp | grep 8080
```

## 💾 10. Check disk space

```bash
df -h
```

## 📦 11. Check directory size

```bash
du -sh /var/log
```

## 🧠 12. Check memory

```bash
free -h
```

## 🖥️ 13. Check CPU

```bash
lscpu
```

## 🌍 14. Test connectivity

```bash
ping -c 4 google.com
```

## 🔎 15. Check DNS

```bash
nslookup google.com
```

## 🔐 16. Check permissions

```bash
ls -l application.log
```

## 👑 17. Change ownership

```bash
sudo chown ubuntu:ubuntu application.log
```

## 🔧 18. Make a script executable

```bash
chmod +x deploy.sh
```

## 🔎 19. Find configuration files

```bash
find /etc -type f -name "*.conf"
```

## 💾 20. Find large files

```bash
find /var -type f -size +100M
```

## 🕒 21. Find recently modified files

```bash
find . -type f -mmin -20
```

## 📥 22. Download a file

```bash
wget https://example.com/app.tar.gz
```

---

# 🧠 Real-World Linux Troubleshooting Flow

```text
                    🚨 SERVER ISSUE
                          │
                          ▼
                    👤 Check User
                        whoami
                          │
                          ▼
                  📂 Check Directory
                         pwd
                          │
                          ▼
                    📋 List Files
                        ls -la
                          │
                          ▼
                  ⚙️ Check Processes
                        ps aux
                          │
                          ▼
                     📜 Check Logs
                        tail -f
                          │
                          ▼
                    🔎 Search Errors
                         grep
                          │
                          ▼
                  💻 Check Resources
                    /             \
                   /               \
               df -h              free -h
                   \               /
                    \             /
                     ▼           ▼
                      🌐 Network
                     ss / ping
                          │
                          ▼
                    🔐 Permissions
                        ls -l
                          │
                          ▼
                       ✅ FIX
```

---

# ⭐ Commands to Master for DevOps

| Category | Commands | Priority |
|---|---|:---:|
| 📂 Navigation | `pwd`, `ls`, `cd` | ⭐⭐⭐ |
| 📁 Files | `mkdir`, `touch`, `cp`, `mv`, `rm` | ⭐⭐⭐ |
| 📖 Reading | `cat`, `head`, `tail`, `tail -f` | ⭐⭐⭐ |
| 🔍 Searching | `find`, `grep`, `locate` | ⭐⭐⭐ |
| 📍 Location | `which`, `whereis` | ⭐⭐ |
| ⚙️ Processes | `ps`, `top`, `kill` | ⭐⭐⭐ |
| 💾 Storage | `df`, `du` | ⭐⭐⭐ |
| 🧠 System | `free`, `lscpu`, `vmstat` | ⭐⭐ |
| 🔐 Permissions | `chmod`, `chown`, `sudo` | ⭐⭐⭐ |
| 👤 Users | `whoami`, `useradd`, `passwd`, `su` | ⭐⭐ |
| 🌐 Networking | `ping`, `nslookup`, `ss`, `hostname` | ⭐⭐⭐ |
| 📥 Downloads | `wget` | ⭐⭐ |
| 📦 Archives | `zip`, `unzip` | ⭐⭐ |
| 🔤 Text | `sort`, `cut`, `tr`, `diff` | ⭐⭐ |
| 🔗 Pipes | `\|` | ⭐⭐⭐ |
| 🕘 History | `history`, `!!`, `!number` | ⭐⭐ |
| 🌱 Environment | `printenv`, `export`, `$PATH` | ⭐⭐⭐ |
| 🧩 Aliases | `alias`, `source` | ⭐⭐ |
| 🔀 Operators | `;`, `&&`, `\|\|`, `&` | ⭐⭐⭐ |
| 🏃 Jobs | `jobs`, `bg`, `fg` | ⭐⭐ |
| 🔑 Encoding | `base64` | ⭐⭐ |

---

# 🏆 Essential Linux Command Set

```text
📂 Navigation
    pwd
    ls
    ls -la
    cd
    cd ..
    cd ~
    cd -

📁 Files & Directories
    mkdir
    mkdir -p
    touch
    cat
    cp
    mv
    rm
    rm -r

📖 File Viewing
    head
    tail
    tail -f

🔍 Searching
    find
    grep
    locate
    which
    whereis

⚙️ Processes
    ps aux
    top
    kill

💾 System
    df -h
    du -sh
    free -h
    lscpu
    uname -a
    vmstat
    lsof

👤 Users
    whoami
    useradd
    passwd
    su

🔐 Permissions
    chmod
    chown
    sudo

🌐 Networking
    ping
    nslookup
    hostname
    ss
    netstat
    wget

📦 Archives
    zip
    unzip

🔤 Text Processing
    echo
    sort
    cut
    tr
    diff

🔗 Pipes & Operators
    |
    ;
    &&
    ||
    &

🕘 History
    history
    !!
    !<number>

🌱 Environment
    printenv
    export
    echo $PATH
    echo $HOME
    source

🧩 Aliases
    alias
    source ~/.bashrc

🏃 Jobs
    jobs
    bg
    fg

🔑 Encoding
    base64
```

---

# 🎯 Linux → DevOps

```text
                     🐧 LINUX
                        │
        ┌───────────────┼────────────────┐
        │               │                │
        ▼               ▼                ▼
    📁 Files        ⚙️ Processes      🌐 Network
        │               │                │
    find / grep      ps / top / kill   ping / ss
        │               │                │
        └───────────────┼────────────────┘
                        │
                        ▼
                  🔐 Permissions
                   chmod / chown
                        │
                        ▼
                 🌱 Environment
                  export / PATH
                        │
                        ▼
                  🔗 Bash / Shell
                  Pipes / Operators
                        │
                        ▼
                       Git
                        │
                        ▼
                       AWS
                        │
                        ▼
                     Docker
                        │
                        ▼
                   Kubernetes
                        │
                        ▼
                     Ansible
                        │
                        ▼
                Prometheus + Grafana
```

---

# 💡 Key Takeaways

- 🐧 Linux is the foundation of many DevOps environments.
- 📂 Learn navigation and file management first.
- 🔎 Master `grep` and `find` for troubleshooting.
- 📜 Learn `tail -f` for real-time log monitoring.
- ⚙️ Understand processes using `ps`, `top` and `kill`.
- 💾 Monitor resources with `df`, `du`, `free` and `lscpu`.
- 🔐 Understand `chmod`, `chown` and `sudo`.
- 🌐 Learn `ping`, `nslookup` and `ss` for networking.
- 🔗 Master pipes and operators for powerful command combinations.
- 🌱 Understand environment variables before working with deployments.
- 🚀 Practice these commands on real servers and cloud instances.

---

<div align="center">

# 🐧 Master Linux → Master DevOps

### Learn the command → Understand the output → Solve the problem

**Linux → Git → AWS → Docker → Kubernetes → Ansible → Monitoring**

---

# 🏁 LINUX COMMANDS COMPLETE

</div>
