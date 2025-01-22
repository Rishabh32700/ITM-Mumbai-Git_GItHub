
## Day 1: Fundamentals of Git and GitHub

### Lecture 2: Understanding Git Basics
#### Theory Notes:
- **Key Components:**
  - **Working Directory**: The local directory where files are being worked on.
  - **Staging Area**: Files added here are prepared for the next commit.
  - **Commit**: A snapshot of the current state of the project.

- **.gitignore:**
  - A file used to specify untracked files that Git should ignore.
  - Example: Ignoring log files, temporary files, etc.

#### Practical Steps:
1. **Add Files to Staging:**
   - Create a sample file:
     ```bash
     echo "Hello, Git!" > example.txt
     ```
   - Add it to the staging area:
     ```bash
     git add example.txt
     ```

2. **Commit Changes:**
   - Save changes to the repository:
     ```bash
     git commit -m "Initial commit with example.txt"
     ```

3. **Create a .gitignore File:**
   - Add entries to `.gitignore` to ignore specific files:
     ```
     *.log
     temp/
     ```
   - Save the file and ensure Git respects it.
