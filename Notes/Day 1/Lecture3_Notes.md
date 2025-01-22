
## Day 1: Fundamentals of Git and GitHub

### Lecture 3: Exploring Commit History and Branching
#### Theory Notes:
- **Viewing Commit History:**
  - Use `git log` to see past commits.
  - Options: `--oneline` for a concise view.

- **Branching:**
  - Branching allows independent development paths.
  - Default branch is usually `main` or `master`.

#### Practical Steps:
1. **View Commit History:**
   ```bash
   git log
   git log --oneline
   ```

2. **Create and Switch Branches:**
   - Create a new branch:
     ```bash
     git branch feature-branch
     ```
   - Switch to the new branch:
     ```bash
     git checkout feature-branch
     ```

3. **Rename a Branch:**
   - Rename the current branch:
     ```bash
     git branch -m new-branch-name
     ```

4. **List Branches:**
   ```bash
   git branch
   ```