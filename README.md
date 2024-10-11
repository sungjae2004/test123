# test123

Version Control and Collaboration  
Version control systems (VCS) manage changes to files over time. They allow multiple people to collaborate on projects, track changes, and restore previous versions of the code when necessary.

Changes vs. Snapshots  
- **Changes**: Track only the differences between file versions.  
- **Snapshots**: Capture the entire state of a project at a specific point in time.  

Local, Centralized, and Distributed Version Control  
- **Local Version Control**: Stores version history on a local machine.  
- **Centralized Version Control**: A central server holds the codebase, and multiple users access it.  
- **Distributed Version Control**: Every user has a full copy of the repository and can work independently, syncing with others later.  

Three States in Git  
1. **Modified**: The file has been changed but not staged.  
2. **Staged**: The changes are marked to be included in the next commit.  
3. **Committed**: The changes have been saved to the local repository.  

### Installing Git  
Git can be installed on various operating systems, including Linux, Mac, and Windows. Below are the installation instructions for each platform.

#### Linux Installation  
To install Git on a Linux distribution, you can use the package manager specific to your distribution. For example, on Debian/Ubuntu, run the following commands in the terminal:

```bash
sudo apt update  
sudo apt install git
```

### Git Config: First-time Setup  
Git can be configured at three levels: system, global, and local.  
- **System level**: Configurations apply to all users on the machine.  
  ```bash
  git config --system user.name "Your Name"
  ```
- **Global level**: Configurations apply only to the current user.  
  ```bash
  git config --global user.name "Your Name"
  ```
- **Local level**: Configurations apply only to a specific repository.  
  ```bash
  git config --local user.name "Your Name"
  ```

### Initializing a Repository  
To initialize a Git repository in an existing directory, use the following command:  
```bash
git init
```

### Checking Repository Status  
To check the current status of your repository, use:  
```bash
git status
```

### Adding Files to Staging Area  
- To stage a specific file for the next commit:  
  ```bash
  git add [file_name]
  ```
- To stage all files in the current directory:  
  ```bash
  git add .
  ```

### Unstaging a File  
To unstage a file that has been staged:  
```bash
git rm --cached [file_name]
```

### Ignoring Files  
To prevent Git from tracking certain files, create a `.gitignore` file and list the file names or patterns you want to ignore.  
Example to ignore all log files:  
```bash
*.log
```

### Committing Changes  
To save your staged changes to the repository with a message describing the changes:  
```bash
git commit -m "Commit message"
```

### Renaming a Branch  
If you want to rename an existing branch:  
```bash
git branch -m [old_branch_name] [new_branch_name]
```
