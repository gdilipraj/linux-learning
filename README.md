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

### 📁 Directory Management `mkdir`
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
The `mv` command is a two-in-one tool. It is used to move files to different folders and is also the standard way to rename files in Linux.

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
It is used to remove files and directories. Warning: In Linux, this is permanent and there is no "Recycle Bin."

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
In Linux, the `>` symbol acts like a funnel. It tells the system: "Take the output from the command on the left and pour it into the file on the right." Note: This will overwrite any existing content in the file.
| Command | Action | Description |
| :--- | :--- | :--- |
| `>` | Redirection |	Redirects output to a file (overwrites existing content). |


**Example Usage:**
```bash
echo "Hello Linux" > myfile.txt
``` 

### 📖 Reading File Content `less`
To view the contents of a file directly in your terminal without opening an editor, you can use the `less` command. It is great for reading large files because it allows you to scroll up and down.

| Command | Action | Description |
| :--- | :--- | :--- |
| `less` | Read File |	Opens a file for interactive reading in the terminal. |

**Example Usage:**
```bash
less myfile.txt
``` 

### 💻 System Information `uname`
The `uname` command is used to display essential details about your operating system and hardware. It is the quickest way to identify the system you are working on.

| Command | Action | Description |
| :--- | :--- | :--- |
| `uname` | System Info	| Displays the operating system name. |
| `uname -a` |	All Info |	Shows detailed kernel version, processor type, and OS details. |

**Example Usage:**
```bash
uname -a
``` 

### 🐱 Concatenate Files `cat`
The `cat` command is one of the most frequently used tools in Linux. While its primary job is to display the entire content of a file to the terminal, it is also used to combine multiple files into one.

| Command | Action | Description |
| :--- | :--- | :--- |
| `cat` |	Read Content | Displays the full content of a file in the terminal. |
| `cat file1 file2` |	Combine Files |	Displays the content of multiple files sequentially. |

**Example Usage:**
```bash
# To view a file's content
cat myfile.txt

# To combine two files into a new one
cat file1.txt file2.txt > combined.txt
``` 

### 🔗 Linking Files `ln`
The ln command is used to create links (shortcuts) between files. This is useful for accessing the same file from different locations without making multiple copies.

| Command | Action | Description |
| :--- | :--- | :--- |
| `ln -s` |	Soft Link |	Creates a symbolic link (shortcut) to a file or folder. |
| `ln` | Hard Link |	Creates a direct link to the data on the disk. |

### 💡 Soft Links vs. Hard Links
Soft Link `-s`: The most common type. It acts like a Windows shortcut; if you delete the original file, the link breaks.

Hard Link: A direct pointer to the file's data. If you delete the original file, the hard link still works.

**Example Usage:**
```bash
# To create a soft link (shortcut)
ln -s original_file.txt shortcut_link

# To create a hard link
ln original_file.txt hard_link
``` 

### 📝 Terminal Text Editor `nano`

The nano command opens a simple, user-friendly text editor directly inside your terminal. It is perfect for making quick changes to configuration files or writing scripts without leaving the command line.



