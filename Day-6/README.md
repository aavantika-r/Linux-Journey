# Day 6 – Linux `find` Command

## 🎯 Objective
Learn how to search files and directories using the `find` command.

---

## 1. Find all .log files

```bash
find /var/log -type f -name "*.log"
```

- `/var/log` → Search path
- `-type f` → Files only
- `-name "*.log"` → Match `.log` files

---

## 2. Find large log files (>100 MB)

```bash
find /var/log -type f -size +100M
```

`+100M` = Files larger than 100 MB.

---

## 3. Find empty files

```bash
find . -type f -empty
```

- `.` → Current directory
- `-empty` → Empty files only

---

## 4. Find old logs

```bash
find /var/log -type f -name "*.log" -mtime +7
```

`-mtime +7` = Not modified for more than 7 days.

---

## 5. Execute a command with `-exec`

```bash
find . -type f -name "*.log" -exec ls -lh {} \;
```

- `-exec` → Execute command
- `ls -lh` → Show size & details
- `{}` → Each matched file
- `\;` → End execution

---

## 📌 Key Options

| Option | Purpose |
|---------|---------|
| `-type f` | Files only |
| `-name` | Search by name |
| `-size` | Search by size |
| `-empty` | Empty files |
| `-mtime` | Modified days |
| `-exec` | Execute command |

---

## 💡 Summary

The `find` command helps locate files using different filters such as **name, type, size, age, and actions**.
