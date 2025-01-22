# Lecture 3: Exploring Commit History and Branching

---

## Exploring Commit History

### **1. Understanding Commit History**
- **Definition**: Commit history is the record of all the changes made to a repository over time, helping developers understand how the project evolved.
- **Why It’s Important**:
  - Tracks changes and reasons for those changes.
  - Identifies contributors to specific features or fixes.
  - Useful for debugging by pinpointing when a bug was introduced.

### **2. The `git log` Command**
- **Basic Usage**:
  ```bash
  git log
  ```
  Displays a detailed history of commits, including:
  - Commit hash: A unique identifier for the commit.
  - Author: The person who made the changes.
  - Date: When the changes were committed.
  - Commit message: A short description of the changes.

- **Modifiers for Better Insights**:
  - `--oneline`: Summarized history with one commit per line.
    ```bash
    git log --oneline
    ```
  - `--graph`: Shows a visual representation of the branching structure.
    ```bash
    git log --graph --oneline
    ```
  - `--since` and `--until`: Filters commits by date range.
    ```bash
    git log --since="2025-01-01" --until="2025-01-22"
    ```
  - `-p`: Shows differences introduced in each commit.
    ```bash
    git log -p
    ```
  - `-n <number>`: Limits the output to the most recent `<number>` commits.
    ```bash
    git log -n 5
    ```

### **3. Exploring a Specific Commit**
- View the full details of a specific commit using:
  ```bash
  git show <commit-hash>
  ```
- Provides:
  - Commit metadata (author, date, etc.).
  - Detailed changes in the commit.

---

## Branching in Git

### **1. What is a Branch?**
- A branch in Git is essentially a pointer to a specific commit.
- It allows developers to work on features, fixes, or experiments in isolation without affecting the main codebase.

### **2. Benefits of Using Branches**
- **Parallel Development**:
  - Multiple developers or teams can work on separate features simultaneously.
- **Safe Experimentation**:
  - Changes can be made and tested on a branch without disrupting the main branch.
- **Easier Collaboration**:
  - Each contributor can work on their branch, merging changes when ready.

### **3. Types of Branches**
- **Default Branch**:
  - Typically named `main` or `master`.
- **Feature Branches**:
  - Used for developing specific features.
  - Example: `feature/login-page`.
- **Hotfix Branches**:
  - Created to fix urgent bugs.
  - Example: `hotfix/critical-bug`.

### **4. Branching Workflows**
- **Feature Branch Workflow**:
  - Each feature gets its branch, and changes are merged into the main branch after completion.
- **Gitflow Workflow**:
  - A structured branching model with dedicated branches for development, release, and hotfixes.

### **5. Visualizing Branches**
- Use `git log --graph --oneline` to see a graphical representation of branches and commits.

---

## Practical Steps

### **1. Viewing Commit History**
1. **Basic History**:
   ```bash
   git log
   ```
   - Observe details like commit hashes, authors, and dates.

2. **Summarized History**:
   ```bash
   git log --oneline
   ```
   - Each commit is displayed in a single line.

3. **Graphical View**:
   ```bash
   git log --graph --oneline
   ```
   - Displays the branching structure.

4. **Filtering Commits**:
   ```bash
   git log --since="2025-01-01"
   git log --until="2025-01-22"
   ```

5. **Inspecting Changes**:
   ```bash
   git log -p
   ```
   - Shows code differences introduced in each commit.

---

### **2. Creating and Renaming Branches**
1. **Create a New Branch**:
   ```bash
   git branch feature/new-feature
   ```

2. **Verify Branch Creation**:
   ```bash
   git branch
   ```

3. **Rename a Branch**:
   - While on the branch to rename:
     ```bash
     git branch -m new-branch-name
     ```

4. **List All Branches**:
   ```bash
   git branch
   ```

---

### **3. Switching Between Branches**
1. **Switching Using `switch`**:
   ```bash
   git switch <branch-name>
   ```
   Example:
   ```bash
   git switch feature/new-feature
   ```

2. **Switching Using `checkout`**:
   ```bash
   git checkout <branch-name>
   ```
   Example:
   ```bash
   git checkout main
   ```

3. **Check Active Branch**:
   ```bash
   git branch
   ```

4. **Test Isolation**:
   - Modify a file and commit changes on one branch.
   - Switch to another branch and observe that the changes are not reflected there.

------------------------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------

## Interview Questions and Answers

1. **What is the purpose of using branches in Git?**
   - **Answer**: Branches in Git allow developers to work on features or fixes in isolation, preventing changes from affecting the main codebase. This enables parallel development, experimentation, and safer collaboration.

2. **How can you visualize the branching structure in a Git repository?**
   - **Answer**: You can visualize the branching structure using the command `git log --graph --oneline`. This shows the commit history along with a graphical representation of branches.

3. **Explain the difference between `git switch` and `git checkout`.**
   - **Answer**: 
     - `git switch` is specifically designed for switching branches.
     - `git checkout` is a more general command used for both switching branches and checking out files. 
     - `switch` is more intuitive for branch operations and is recommended for modern Git usage.

4. **How would you rename a branch in Git?**
   - **Answer**: To rename a branch, use the command `git branch -m <new-branch-name>` while on the branch you want to rename.

5. **What does the `git log --since` and `git log --until` command do?**
   - **Answer**: These options allow you to filter the commit history based on a date range. 
     - `--since` shows commits after the specified date.
     - `--until` shows commits before the specified date.

---

## Multiple Choice Questions (MCQs)

1. **Which command is used to create a new branch in Git?**
   - A) `git branch new-branch`
   - B) `git create-branch new-branch`
   - C) `git switch new-branch`
   - D) `git checkout -b new-branch`
   
   <details>
     <summary>Answer</summary>
     A) `git branch new-branch`
   </details>

2. **How can you summarize the commit history in a single line per commit?**
   - A) `git log --summary`
   - B) `git log --compact`
   - C) `git log --oneline`
   - D) `git log --short`
   
   <details>
     <summary>Answer</summary>
     C) `git log --oneline`
   </details>

3. **What is the default branch created in a new Git repository?**
   - A) `main`
   - B) `master`
   - C) `default`
   - D) `branch`
   
   <details>
     <summary>Answer</summary>
     A) `main` (in newer versions of Git) or B) `master` (in older versions).
   </details>

4. **How do you check which branch you are currently on?**
   - A) `git show branch`
   - B) `git branch`
   - C) `git status`
   - D) `git show current-branch`
   
   <details>
     <summary>Answer</summary>
     B) `git branch`
   </details>

5. **What happens if you try to commit changes in Git without configuring your user name and email?**
   - A) Git will commit with a default name and email.
   - B) The commit will fail without any message.
   - C) Git will throw an error and prevent the commit.
   - D) Git will assign a random user name and email to the commit.
   
   <details>
     <summary>Answer</summary>
     C) Git will throw an error and prevent the commit.
   </details>