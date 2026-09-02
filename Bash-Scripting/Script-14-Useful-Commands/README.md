# 🐚 Bash — Useful Commands

### 🔹 `grep` — Search Text

```bash
grep "error" logfile.txt
```

- Searches for specific text inside a file.

### 🔹 `awk` — Process Text

```bash
awk '{print $1}' users.txt
```

- Extracts and processes columns from text.

### 🔹 `sort` — Sort Output

```bash
sort names.txt
```

- Sorts lines alphabetically.

### 🔹 `uniq` — Remove Duplicates

```bash
sort names.txt | uniq
```

- Removes duplicate lines.

### 🔹 `wc` — Count

```bash
wc -l file.txt
```

- Counts the number of lines in a file.

### 🔹 `curl` — Test URLs

```bash
curl https://example.com
```

- Sends a request to a URL and displays the response.

### 💡 Key Idea

```text
grep → Search
awk  → Process
sort → Sort
uniq → Remove duplicates
wc   → Count
curl → Test URLs / APIs
```

> 🚀 These commands are commonly used in **DevOps, Linux administration, log analysis, and automation**.
