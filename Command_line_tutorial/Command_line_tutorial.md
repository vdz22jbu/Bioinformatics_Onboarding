## Command Line Basics Tutorial (Beginner - Windows Git Bash - 10 minutes)

Welcome! You're now in your terminal with Git Bash open. This tutorial will teach you the essentials of navigating and managing files via the command line.

### 1. Know Where You Are: `pwd` (Print Working Directory)
Your first question should always be: "Where am I?" Type this command:
```bash
pwd
```
This shows your current location as a path (e.g., `/c/Users/bjw37/Desktop`). You'll use `pwd` frequently to orient yourself.

### 2. See What's Around You: `ls` (List)
Now see what files and folders are in your current location:
```bash
ls
```
Add a flag to see more details:
```bash
ls -la
```
The `-l` flag shows long format (with permissions, size, date). The `-a` flag shows hidden files too. Flags modify how commands behave.

### 3. Navigate Directories: `cd` (Change Directory)
Move into a folder using:
```bash
cd Documents
```
Check where you are now:
```bash
pwd
```
Move back up one level:
```bash
cd ..
```
Move to your home directory from anywhere:
```bash
cd ~
```
Or simply:
```bash
cd
```

### 4. Tab Completion (Your Best Friend!)
Start typing a folder or file name and press **Tab** to auto-complete. For example:
```bash
cd Doc[TAB]
```
Git Bash will complete it to `cd Documents`. This saves time and prevents typos. If multiple matches exist, press Tab twice to see options.

### 5. Create a New Directory: `mkdir` (Make Directory)
```bash
mkdir my_project
```
Now navigate into it:
```bash
cd my_project
```

### 6. Create a New File: `touch`
```bash
touch my_file.txt
```
Check it exists:
```bash
ls
```

### 7. Copy Files: `cp` (Copy)
```bash
cp my_file.txt my_file_copy.txt
```
Copy into another directory:
```bash
cp my_file.txt ../my_file.txt
```

### 8. Move or Rename Files: `mv` (Move)
Rename a file:
```bash
mv my_file_copy.txt backup.txt
```
Move it to another directory:
```bash
mv backup.txt ../backup.txt
```

### 9. Remove Files: `rm` (Remove)
**Warning: This is permanent!**
```bash
rm my_file.txt
```
Remove a directory (only if empty):
```bash
rmdir my_folder
```
Remove a directory and everything inside it:
```bash
rm -r my_folder
```
The `-r` flag means "recursive" (go through all contents).

### 10. Get Help: `--help` or `man`
Confused about a command? Use the `--help` flag:
```bash
ls --help
```
This shows all available flags and options. For more detailed help (on Mac/Linux HPC systems):
```bash
man ls
```
(Press `q` to quit the manual.)

### Practice Exercise
Try this sequence to reinforce what you learned:
```bash
pwd                                    # Where am I?
cd ~                                   # Go home
mkdir command_line_practice            # Create a practice folder
cd command_line_practice               # Enter it
touch file1.txt file2.txt              # Create two files
ls                                     # List them
cp file1.txt file1_backup.txt          # Copy one
mv file2.txt file2_renamed.txt         # Rename one
ls -la                                 # List with details
rm file1_backup.txt                    # Delete the backup
pwd                                    # Where are you now?
cd ..                                  # Go back up
rm -r command_line_practice            # Clean up (removes the whole folder)
```

### Key Takeaways
- **`pwd`** to know where you are
- **`ls`** to see what's there
- **`cd`** to navigate
- **Tab** to auto-complete
- **`mkdir`** to create folders
- **`touch`** to create files
- **`cp`**, **`mv`**, **`rm`** to manage files
- **Flags** (like `-la`, `-r`) to modify command behavior
- **`--help`** when you're stuck

You now have the foundation to navigate your file system from the command line! As you progress through this course, you'll build on these basics to run bioinformatics tools, manage data, and work on remote servers.
