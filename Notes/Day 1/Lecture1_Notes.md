## Day 1: Fundamentals of Git and GitHub

### Lecture 1: Introduction to Version Control
#### Theory Notes:
- **What is Version Control?**
  - Version Control is a system that records changes to a file or set of files over time.
  - It allows you to revisit specific versions later, compare changes, and collaborate effectively.
  - Examples: Git, SVN, Mercurial.

- **Benefits of Version Control:**
  - Keeps a history of changes.
  - Facilitates team collaboration.
  - Simplifies branching and merging workflows.

- **Git vs Other VCS:**
  - Git is distributed, meaning every user has a complete copy of the repository.
  - Other VCS, like SVN, often rely on a central server.

#### Practical Steps:
1. **Install Git:**
   - Download Git from [git-scm.com](https://git-scm.com/).
   - Install using default settings.
   - Verify installation:
     ```bash
     git --version
     ```

2. **Configure Git:**
   - Set global user name and email:
     ```bash
     git config --global user.name "Your Name"
     git config --global user.email "your_email@example.com"
     ```

3. **Initialize a Repository:**
   - Create a new directory and navigate to it:
     ```bash
     mkdir my_project && cd my_project
     ```
   - Initialize Git:
     ```bash
     git init
     ```