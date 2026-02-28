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

### 🚀 Directory Navigation `cd`

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

### ✍️ File Creation `touch`
The `touch` command was originally meant to update the timestamp of a file, but if the file does not exist, Linux creates a blank one.

| Command | Action | Description |
| :--- | :--- | :--- |
| `touch` | Create / Update |	Creates a blank file or updates the timestamp of an existing one. |

**Example Usage:**
``` bash
touch my_new_file.txt
```


### 🚚 Moving & Renaming `mv`
The mv command is a two-in-one tool. It is used to move files to different folders and is also the standard way to rename files in Linux.

| Command | Action | Description |
| :--- | :--- | :--- |
| `mv` | Move / Rename | Relocates or changes the name of files and folders. |

**Example 1: Renaming a file**
``` bash
mv  old_filename.txt   new_filename.txt
```

**Example 2: Moving a file into a folder**
``` bash
mv  file.txt   folder_name/
```


### 👯 Copying Files `cp`
Use this command to create a duplicate of a file or directory in a different location.

| Command | Action | Description |
| :--- | :--- | :--- |
| `cp` | Copy |	Duplicates files or directories to a new path. |

**Example Usage:**
```bash
cp file.txt copy_of_file.txt
``` 

### 🗑️ Deleting Files `rm`
This is used to remove files and directories. Warning: In Linux, this is permanent and there is no "Recycle Bin."

| Command | Action | Description |
| :--- | :--- | :--- |
| `rm` | Remove	| Deletes files or directories permanently from the system. |

**Example Usage:**
```bash
# To delete a file
rm file.txt

# To delete a folder (recursive)
rm -r folder_name
```

### 🖋️ File Redirection `>`
In Linux, the > symbol acts like a funnel. It tells the system: "Take the output from the command on the left and pour it into the file on the right." Note: This will overwrite any existing content in the file.
| Command | Action | Description |
| :--- | :--- | :--- |
| `>` | Redirection |	Redirects output to a file (overwrites existing content). |


**Example Usage:**
```bash
echo "Hello Linux" > myfile.txt
``` 

### 📖 Reading File Content (less)
To view the contents of a file directly in your terminal without opening an editor, you can use the less command. It is great for reading large files because it allows you to scroll up and down.




















