
# Lecture 1: Introduction to Version Control

## Theory Notes

### 1. What is Version Control?
**Definition**:  
Version control is a system that helps you manage changes to files over time. It allows you to:  
- Track the history of changes.  
- Collaborate with others on the same project without overwriting each other's work.  
- Restore previous versions of your files if needed.  

**Why it Matters**:  
- In team projects, version control ensures everyone works seamlessly, even on the same files.  
- It acts like an "undo" button for your project's history.  

**Real-Life Analogy**:  
Imagine writing a group essay. Without version control, everyone might overwrite each other's edits. With version control, you can:  
- Track who made what changes and when.  
- Revert to an earlier draft if needed.  
- Merge everyone's contributions without conflicts.  

---

### 2. Benefits of Version Control
- **Collaboration**: Multiple people can work on the same project at the same time.  
- **History Tracking**: You can see a detailed log of who made changes, when, and why.  
- **Backup and Recovery**: Easily roll back to previous versions of a file or project.  
- **Experimentation**: Try out new features or changes without affecting the main project (using branching).  
- **Consistency**: Helps maintain a stable codebase by tracking every change.  

---

### 3. Comparison: Git vs Other VCS (e.g., SVN)
| **Feature**       | **Git (Distributed)**                           | **SVN (Centralized)**               |
|--------------------|-------------------------------------------------|--------------------------------------|
| **Architecture**  | Distributed: Every user has a full copy of the repository. | Centralized: Relies on a central server. |
| **Speed**         | Faster: Operations are mostly local.            | Slower: Operations depend on the central server. |
| **Offline Work**  | Full functionality offline.                     | Limited functionality offline.       |
| **Branching**     | Easy and lightweight.                           | Heavy and slower.                    |
| **Collaboration** | Allows peer-to-peer collaboration.              | Requires central server coordination.|

---

## Practical Steps

### 1. Install Git Locally
**Download Git**:  
- Go to [Git's official website](https://git-scm.com/).  
- Download the installer suitable for your operating system (Windows, macOS, or Linux).  

**Install Git**:  
- Follow the installation prompts.  
- For Windows: Choose to add Git to your system’s PATH for easier command-line access.  

**Verify Installation**:  
1. Open a terminal or command prompt.  
2. Run the command:  
   ```bash
   git --version
   ```  
3. You should see the installed version of Git.  

---

### 2. Configure Global and Local Settings
**Global Settings**: These apply to all repositories on your machine.  
1. Set your name:  
   ```bash
   git config --global user.name "Your Name"
   ```  
2. Set your email (used for commit authorship):  
   ```bash
   git config --global user.email "your_email@example.com"
   ```  
3. Verify configuration:  
   ```bash
   git config --list
   ```  

**Local Settings**: These apply to a specific repository.  
1. Navigate to your project folder:  
   ```bash
   cd /path/to/your/project
   ```  
2. Set repository-specific name and email:  
   ```bash
   git config user.name "Project-Specific Name"
   git config user.email "project_email@example.com"
   ```  

---

### 3. Initialize a Git Repository
1. **Create a New Directory**:  
   Run the command:  
   ```bash
   mkdir my_project && cd my_project
   ```  

2. **Initialize Git**:  
   Turn the directory into a Git repository:  
   ```bash
   git init
   ```  
   You will see the response:  
   ```bash
   Initialized empty Git repository in /path/to/my_project/.git/
   ```  

3. **Verify Initialization**:  
   Check the presence of the `.git` folder:  
   ```bash
   ls -a
   ```  
   You should see `.git`, indicating the directory is now a Git repository.  
