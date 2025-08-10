# Let's create a comprehensive Bash commands cheatsheet in README format
bash_cheatsheet = """# 🐚 Bash Command Cheatsheet

A handy collection of **basic to advanced Bash commands** that a senior engineer often uses.

---

## 📌 Basic Navigation & File Management

| Command | Description |
|---------|-------------|
| `pwd` | Print current working directory |
| `ls` | List files and directories |
| `ls -la` | List all files with details |
| `cd <dir>` | Change directory |
| `cd ..` | Move up one directory |
| `cd -` | Switch to previous directory |
| `touch <file>` | Create an empty file |
| `mkdir <dir>` | Create a directory |
| `mkdir -p a/b/c` | Create nested directories |
| `rm <file>` | Remove file |
| `rm -r <dir>` | Remove directory recursively |
| `rm -rf <dir>` | Force remove directory recursively |
| `cp <src> <dest>` | Copy file |
| `cp -r <src> <dest>` | Copy directory recursively |
| `mv <src> <dest>` | Move or rename file/directory |

---

## 📌 Viewing & Editing Files

| Command | Description |
|---------|-------------|
| `cat <file>` | Display file content |
| `less <file>` | View file with scrolling |
| `head <file>` | Show first 10 lines |
| `head -n 20 <file>` | Show first 20 lines |
| `tail <file>` | Show last 10 lines |
| `tail -n 50 <file>` | Show last 50 lines |
| `tail -f <file>` | Follow log output |
| `nano <file>` | Edit file in Nano |
| `vim <file>` | Edit file in Vim |

---

## 📌 Searching & Finding

| Command | Description |
|---------|-------------|
| `find . -name "*.txt"` | Find files matching pattern |
| `grep "text" file` | Search for text in file |
| `grep -r "text" .` | Search recursively in directory |
| `grep -i "text" file` | Case-insensitive search |
| `grep -n "text" file` | Show line numbers in search |
| `history` | Show command history |
| `!!` | Run last command |
| `!<number>` | Run command from history by number |

---

## 📌 Permissions & Ownership

| Command | Description |
|---------|-------------|
| `chmod 755 <file>` | Change file permissions |
| `chmod +x <file>` | Make file executable |
| `chown user:group <file>` | Change file owner and group |

---

## 📌 Networking

| Command | Description |
|---------|-------------|
| `curl <url>` | Fetch content from URL |
| `wget <url>` | Download file from URL |
| `ping <host>` | Check connectivity |
| `ifconfig` | Show network interfaces (Linux) |
| `ip a` | Show IP addresses |
| `netstat -tulpn` | Show active ports |
| `ss -tulpn` | Show active sockets |

---

## 📌 Process Management

| Command | Description |
|---------|-------------|
| `ps aux` | Show running processes |
| `top` | Live process monitor |
| `htop` | Interactive process monitor (if installed) |
| `kill <pid>` | Kill process by PID |
| `kill -9 <pid>` | Force kill process |
| `pkill <name>` | Kill process by name |

---

## 📌 Archives & Compression

| Command | Description |
|---------|-------------|
| `tar -cvf file.tar dir` | Create tar archive |
| `tar -xvf file.tar` | Extract tar archive |
| `tar -czvf file.tar.gz dir` | Create gzip-compressed tar |
| `tar -xzvf file.tar.gz` | Extract gzip-compressed tar |
| `zip file.zip file1 file2` | Create zip archive |
| `unzip file.zip` | Extract zip archive |

---

## 📌 Disk & Storage

| Command | Description |
|---------|-------------|
| `df -h` | Show disk usage |
| `du -sh <dir>` | Show directory size |
| `lsblk` | List block devices |
| `mount` | Show mounted filesystems |

---

## 📌 Environment & Variables

| Command | Description |
|---------|-------------|
| `echo $VAR` | Print variable |
| `export VAR=value` | Set variable |
| `env` | Show environment variables |
| `set` | Show shell variables |
| `unset VAR` | Remove variable |

---

## 📌 Scripting Essentials

| Command | Description |
|---------|-------------|
| `#!/bin/bash` | Shebang for Bash script |
| `for i in {1..5}; do echo $i; done` | Simple loop |
| `if [ -f file ]; then echo "Exists"; fi` | Check if file exists |
| `$(command)` | Command substitution |
| `` `command` `` | Alternate command substitution |

---

## 📌 Useful Shortcuts

| Command | Description |
|---------|-------------|
| `Ctrl + C` | Stop process |
| `Ctrl + Z` | Suspend process |
| `fg` | Resume foreground process |
| `bg` | Resume in background |
| `Tab` | Autocomplete command/file |
| `Ctrl + R` | Reverse search in history |

---

**Pro Tip:** Combine commands with `&&` (run if previous succeeds) or `||` (run if previous fails).  
Example: `mkdir newdir && cd newdir`

"""

# Save to file
bash_cheatsheet_path = "/mnt/data/bash_cheatsheet.md"
with open(bash_cheatsheet_path, "w") as f:
    f.write(bash_cheatsheet_path)

bash_cheatsheet_path
