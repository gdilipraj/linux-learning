# 🐧 My Personal Linux Learning Journey
> "The journey of a thousand miles begins with a single `root` command."

---

### 🌟 The Tradition
Of course, we have to start with the evergreen tradition. This command prints text to your terminal.

```bash
echo "hello world"
```
### 👤 User Identity & Information

| Command | Action | Expected Output |
| :--- | :--- | :--- |
| `whoami` | Identity Check | `gdilipraj` |
| `id` | Group Info | `uid=1000(gdilipraj) gid=1000(gdilipraj) ...` |
| `id root` | Target Check | `uid=0(root) gid=0(root) groups=0(root)` |
| `id -un` | Name Only | `gdilipraj` |

---

### 📂 Navigation & File Discovery

| Command | Action | Expected Output |
| :--- | :--- | :--- |
| `pwd` | Path Check | `/c/Users/desktop` |
| `ls` | List Files | `README.md  linux-learning.md` |
| `ls -l` | Long List | `-rw-r--r-- 1 gdilipraj 1024 Feb 26 23:26 README.md` |
| `ls -la` | Full Detail | `.  ..  .git  README.md  linux-learning.md` |

---

### 🚀 Directory Navigation (`cd`)

| Command | Action | Description |
| :--- | :--- | :--- |
| `cd /` | System Root | Takes you to the very top level of the entire system. |
| `cd ~` | Home Directory | Moves you to your personal user home folder. |
| `cd ..` | Parent Folder | Moves up one level to the parent of your current location. |
| `cd -` | Toggle Folder | Switches back to the previous directory you were in. |

---

### 📁 Directory Management
To create a new directory (folder) in your current location, use the `mkdir` command.

| Command | Action | Description |
| :--- | :--- | :--- |
| `mkdir` | Make Directory | Creates a new folder with the specified name. |

**Example Usage:**
``` bash
mkdir my_new_folder
```
