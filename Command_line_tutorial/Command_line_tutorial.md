## Self-Guided Command Line Tutorial (10 Minutes)

### Quick Overview
In this tutorial, you'll learn the essential commands to navigate your Mac's terminal, manage files and directories, and understand command flags. You're ready to begin since you have VS Code open with a terminal tab.

---

### 1. **Know Where You Are: Print Working Directory (2 minutes)**

Your terminal starts in your home directory. To see your current location:

```bash
pwd
```

**What it does:** "Print Working Directory" shows the full path of where you are in the file system.

**🎯 Try it now:**
- Type `pwd` and press Enter
- You should see something like `/Users/YourUsername`

---

### 2. **List Files: See What's Around You (2 minutes)**

To see what files and folders are in your current directory:

```bash
ls
```

**What it does:** Lists all visible files and folders in your current directory.

**Useful flags:**
- `ls -l` — Shows detailed information (permissions, size, date)
- `ls -a` — Shows ALL files, including hidden ones (starting with `.`)
- `ls -la` — Combines both flags

**🎯 Try it now:**
- Type `ls` and press Enter
- Type `ls -la` and press Enter to see more detail

---

### 3. **Change Directory: Navigate Around (2 minutes)**

Move into a different directory:

```bash
cd Desktop
```

**What it does:** "Change Directory" moves you into the specified folder.

**Navigation tricks:**
- `cd ~` — Go to your home directory
- `cd ..` — Go up one directory level
- `cd -` — Go back to the previous directory
- `cd /` — Go to the root of your system

**🎯 Try it now:**
- Type `pwd` to confirm your location
- Type `cd Desktop` to move to your Desktop folder
- Type `pwd` again to see you moved
- Type `cd ..` to go back to your home directory

---

### 4. **Create a Directory: Make New Folders (1 minute)**

```bash
mkdir my_first_folder
```

**What it does:** "MaKe DIRectory" creates a new folder with the name you specify.

**🎯 Try it now:**
- Type `mkdir my_first_folder` and press Enter
- Type `ls` to see your new folder

---

### 5. **Create a File: Make Empty Files (1 minute)**

```bash
touch my_file.txt
```

**What it does:** Creates an empty file with the name you specify.

**🎯 Try it now:**
- Type `touch my_file.txt` and press Enter
- Type `ls` to see your new file

---

### 6. **Copy Files: Duplicate Content (1 minute)**

```bash
cp my_file.txt my_file_copy.txt
```

**What it does:** "CoPy" copies a file from the first location to create a second file.

**Syntax:** `cp <source> <destination>`

**🎯 Try it now:**
- Type `cp my_file.txt my_file_copy.txt`
- Type `ls` to see both files

---

### 7. **Move (Rename) Files: Relocate Files (1 minute)**

```bash
mv my_file_copy.txt renamed_file.txt
```

**What it does:** "MoVe" relocates a file to a new location or renames it.

**Syntax:** `mv <source> <destination>`

**Examples:**
- `mv my_file.txt my_first_folder/` — Moves file into a folder
- `mv old_name.txt new_name.txt` — Renames a file

**🎯 Try it now:**
- Type `mv my_file_copy.txt renamed_file.txt`
- Type `ls` to confirm the rename

---

### 8. **Remove Files: Delete Content (Carefully!) (0.5 minutes)**

```bash
rm renamed_file.txt
```

**What it does:** "ReMove" deletes a file permanently. **⚠️ There's no undo!**

**Warning:** Don't use `rm -rf` unless you're absolutely certain—it recursively deletes entire folders without asking.

**Safer alternative:**
- Move files to Trash instead: `mv renamed_file.txt ~/.Trash/`

**🎯 Try it now:**
- Type `rm renamed_file.txt`
- Type `ls` to confirm it's gone

---

### 9. **Tab Completion: Type Faster (0.5 minutes)**

Start typing a command or file name and press **Tab** to autocomplete. This saves time and prevents typos.

**🎯 Try it now:**
- Type `my_` and press Tab — it will autocomplete `my_first_folder` if that's the only matching file/folder
- Press **Tab** twice to cycle through suggestions

---

### 10. **Understanding Flags (0.5 minutes)**

Flags modify how commands work. They start with `-` (single flag) or `--` (full name).

**Examples:**
- `ls -a` — The `-a` flag means "show all," including hidden files
- `ls -l` — The `-l` flag means "long format" with details
- `ls -la` — Combine multiple flags (shows all files with details)

**🎯 Try it now:**
- Type `ls -a` to see hidden files
- Type `ls -la` to see details on all files

---

### 11. **Get Help: The `man` Command (0.5 minutes)**

Confused about a command? Use the manual:

```bash
man ls
```

**What it does:** Opens the manual page for the `ls` command. Press `q` to quit.

**Quick help alternative:** Most commands also support `--help`:

```bash
ls --help
```

**🎯 Try it now:**
- Type `man ls` and read a bit
- Press `q` to exit

---

### 12. **Cleanup: Remove Your Test Folder (1 minute)**

Let's clean up what we created:

```bash
rm -r my_first_folder
```

**⚠️ Warning:** The `-r` flag means "recursive"—it deletes the folder AND everything inside. Use carefully!

**🎯 Try it now:**
- Type `rm -r my_first_folder`
- Type `ls` to confirm it's gone

---

### Congratulations! 🎉

You now understand:
- ✅ Where you are (`pwd`)
- ✅ What's around you (`ls`)
- ✅ How to navigate (`cd`)
- ✅ How to create directories and files (`mkdir`, `touch`)
- ✅ How to copy and move files (`cp`, `mv`)
- ✅ How to delete files (`rm`)
- ✅ How to use tab completion
- ✅ How flags modify commands
- ✅ How to get help (`man`, `--help`)

**Next steps:** Practice these commands regularly. They're the foundation for everything you'll do on the command line!

---