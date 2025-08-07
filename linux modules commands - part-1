
# 🧰 LINUX COMMANDS – PART 1

Welcome to the world of Linux command-line tools!  
In this mini-series, we’ll break down some essential commands that every Linux beginner and intermediate user should know.

No long man pages. No jargon dumps. Just clear, practical knowledge.  
If you're using a Linux VM or something like the AttackBox, you're good to go. Let’s dive in!

---

## 📦 1) `du` – *Check Disk Usage Like a Pro*

Ever wondered which files or folders are hogging all your space? That’s where `du` comes in — short for **Disk Usage**.

### 🔍 What Does `du` Do?

`du` gives you a breakdown of how much disk space files and directories are using.  
By default, it summarizes at the directory level (usually in kilobytes), but with a few simple flags, you can make it work magic.

---

### ⚙️ Handy Flags to Remember

| Flag         | What It Does                              |
|--------------|-------------------------------------------|
| `-a`         | Show sizes for individual files too       |
| `-h`         | Human-readable sizes (KB, MB, GB)         |
| `-c`         | Display a grand total at the end          |
| `-d <n>`     | Limit the depth of directory traversal     |
| `--time`     | Show last modified time for entries        |

---

### 🧪 Example Commands

- `du -a /home/`  
  → Lists *everything* in `/home/`, including files, with sizes.

- `du -a /home/ | grep user`  
  → Filters the above to show only items with "user" in the path.

- `du --time -d 1 .`  
  → Shows size and last modification time for current and first-level subfolders.

---

### 📍 Quick Tip  
Want to know **who owns** a file or when it was modified in detail? `du` won’t help with that — use:

```bash
stat <filename>
```

It gives you owner, permissions, timestamps, and more.

---

## 🔎 2) `grep`, `egrep`, `fgrep` – *The Pattern Detectives*

One of the most powerful and frequently used tools in Linux. If you're ever analyzing logs, configs, or outputs — you'll use `grep`.

---

### 🛠️ What’s `grep`?

`grep` searches for patterns in files or input — typically using **regular expressions**.  
It prints only the lines that match, making it super useful for filtering out the noise.

---

### 👪 Meet the Family

- `grep` → Uses **Basic Regular Expressions** (BRE)  
- `egrep` → Same as `grep -E`, for **Extended Regular Expressions**  
- `fgrep` → Same as `grep -F`, searches **fixed strings** (no regex)

---

### 📚 Must-Know Flags

| Flag       | What It Does                                 |
|------------|----------------------------------------------|
| `-R`       | Recursively search through directories       |
| `-i`       | Case-insensitive matching                    |
| `-c`       | Count how many lines matched                 |
| `-n`       | Show line numbers for matches                |
| `-v`       | Invert match: show lines that *don’t* match |
| `-l`       | Print filenames with matches, not the lines  |
| `-h`       | Hide filenames in output (useful in pipes)   |
| `-E`       | Use extended regex (same as `egrep`)         |
| `-F`       | Use fixed string search (same as `fgrep`)    |
| `-e`       | Use multiple patterns in one search          |

---

### 🔍 A Couple of Quick Examples

```bash
grep -i error logs.txt
```
→ Case-insensitive search for “error” in logs.txt

```bash
grep -Rn "192.168" /etc/
```
→ Recursive search for IP patterns in `/etc/`, with line numbers

```bash
grep -Ev '^#|^$' config.conf
```
→ Ignore commented and blank lines from a config file

---

## 🎉 Wrapping Up (For Now…)

If you've made it this far — you're doing amazing. Seriously.  
Commands like `du` and `grep` might seem small, but they’re *power tools* in the real world of Linux.

Once you get comfortable with these, you'll start moving faster, thinking clearer, and debugging better. And we’re just getting started — stay tuned, because next up we’ll tackle `tr`, `awk`, and `sed` in the same clean style.

💡 Every line you run is a step toward real mastery.

---

**Next up: `tr`, `awk`, and `sed` — coming soon!**
