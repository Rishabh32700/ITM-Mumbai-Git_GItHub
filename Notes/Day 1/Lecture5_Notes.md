# **Lecture 5: Introduction to GitHub**

---

## **Introduction**
### Icebreaker Question:
- Ask students: 
  *"How do you currently manage your code or projects? Have you ever collaborated with someone on the same project?"*  
  - Discuss briefly how GitHub simplifies version control and collaboration.

### What is GitHub?
- **GitHub**: A platform for hosting and collaborating on code repositories using Git.
- **Real-world examples**: Companies and open-source projects using GitHub (e.g., Linux, TensorFlow).

---

## **GitHub Basics and Account Setup**

### What is GitHub and Why Use It?
- **Key Features:**
  - Collaboration on code in real-time.
  - Keeping track of code changes (version control).
  - A platform for contributing to open-source projects.
  - Hosting personal projects and portfolios.

- **Why is GitHub Important?**
  - Industry standard for developers.
  - Builds credibility by showcasing projects.
  - Helps teams work together without conflicts in code.

### Account Setup:
1. Create an account on [GitHub](https://github.com).
2. **Plans:**
   - Free: Unlimited public/private repositories.
   - Paid: Advanced tools for professional development.

---

## **GitHub Interface Overview**

### Navigating GitHub Interface:
1. **Dashboard:** Displays recent activity and repositories.
2. **Repositories:** Central place for managing project files.
3. **Pull Requests:** Collaborate on code changes.
4. **Issues Tab:** Track bugs and manage tasks.
5. **Settings:** Manage repository settings and access.

### Repository Types:
- **Public Repository:** Accessible to everyone.
- **Private Repository:** Limited access to collaborators.

---

## **Creating and Managing Repositories**

### Steps to Create a New Repository:
1. Click the **+ icon** (top-right) > **New Repository**.
2. Fill in details:
   - **Name:** Unique identifier for your project.
   - **Description:** Brief overview of the project.
   - **Visibility:** Public or Private.
   - **Initialize with README:** Recommended for beginners.
3. Click **Create Repository**.

### Managing Repository Content:
- **Add Files Manually:** Use the **Add File** button.
- **Using Command Line:** Push files with Git commands.

---

## **Introduction to GitHub Profile README**

### What is a Profile README?
- A personal introduction page on GitHub.
- Highlights skills, projects, and links to other profiles (e.g., LinkedIn).

### Steps to Create a Profile README:
1. Go to **Repositories** > Create a new repository named `<YourUsername>`.
2. Initialize with a README file.
3. Add content using Markdown:
   ```markdown
   ## About Me
   Hi, I'm [Your Name], a software developer specializing in web applications.

   ## Projects
   - [Project Name](Link) - A brief description of the project.

   ## Skills
   - Programming: Python, JavaScript.
   - Tools: Git, Docker.
   ```

---

## **Practical Session**

### **1. Setting Up GitHub Profile**
- Customize profile details:
  - Upload a professional profile picture.
  - Add a bio, location, and website.
  - Link to other platforms (e.g., LinkedIn).

### **2. Creating and Cloning Repositories**

#### Creating a Repository:
1. Follow the steps mentioned above.
2. Add collaborators:
   - Go to **Settings** > **Collaborators and Teams** > Add a collaborator by username or email.

#### Cloning a Repository:
1. Open your repository > Click the **Code** button > Copy the HTTPS link.
2. In your terminal:
   ```bash
   git clone <repository-url>
   ```
3. Verify by listing the folder’s contents.

### **3. Profile README Customization**
1. Edit the README file of the profile repository:
   - Use Markdown to add "About Me" and "Projects."
2. Commit and push changes:
   ```bash
   git add README.md
   git commit -m "Update profile README"
   git push
   ```

### **4. Introduction to Collaboration**

#### Forking a Repository:
1. Fork an open-source repository using the **Fork** button.
2. Clone the forked repository locally.

#### Creating a Pull Request:
1. Make changes in the forked repository.
2. Push changes and create a pull request in the original repository.
3. Describe the changes in the pull request.

------------------------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------

## **Interview Questions and Answers**

1. **What is the difference between Git and GitHub?**  
   - **Answer:**  
     - Git is a version control system that helps manage source code history, while GitHub is a cloud-based hosting platform for Git repositories.  
     - Git is used locally on your machine, while GitHub allows for collaboration, hosting, and sharing code with others.

2. **What is a fork in GitHub, and why is it used?**  
   - **Answer:**  
     - A fork is a copy of a repository that resides in your GitHub account. It is used to make changes to someone else's project without affecting the original repository. You can later contribute back via a pull request.

3. **What are the differences between a `git merge` and a `git rebase`?**  
   - **Answer:**  
     - `git merge` combines changes from two branches and preserves the history of both branches.  
     - `git rebase` applies changes from one branch on top of another, rewriting the commit history to make it linear.

4. **How can you revert a specific commit in Git?**  
   - **Answer:**  
     - You can use the `git revert <commit-hash>` command. This creates a new commit that undoes the changes introduced in the specified commit.

5. **What is the purpose of a .gitignore file?**  
   - **Answer:**  
     - The `.gitignore` file specifies intentionally untracked files that Git should ignore. This is commonly used for files like logs, build artifacts, or sensitive configuration files.

---

## **Multiple-Choice Questions (MCQs)**

1. **What is the primary purpose of GitHub?**  
   - A) File storage for large files  
   - B) A cloud-based hosting platform for Git repositories  
   - C) A replacement for Git as a version control system  
   - D) A database management tool  
   <details>
     <summary>Answer</summary>
     B) A cloud-based hosting platform for Git repositories.
   </details>

---

2. **Which command is used to clone a repository from GitHub to your local machine?**  
   - A) `git copy`  
   - B) `git pull`  
   - C) `git clone`  
   - D) `git fetch`  
   <details>
     <summary>Answer</summary>
     C) `git clone`.
   </details>

---

3. **What is the purpose of a pull request in GitHub?**  
   - A) To merge changes from the main branch to a feature branch  
   - B) To suggest and review changes before merging them into the main branch  
   - C) To delete a repository  
   - D) To upload files to the repository  
   <details>
     <summary>Answer</summary>
     B) To suggest and review changes before merging them into the main branch.
   </details>

---

4. **Which of the following commands initializes a new Git repository?**  
   - A) `git start`  
   - B) `git init`  
   - C) `git config`  
   - D) `git create`  
   <details>
     <summary>Answer</summary>
     B) `git init`.
   </details>

---

5. **What does the `git status` command do?**  
   - A) Displays the commit history of the repository  
   - B) Lists the current branch and untracked files in the repository  
   - C) Stages all changes for commit  
   - D) Merges the current branch with another branch  
   <details>
     <summary>Answer</summary>
     B) Lists the current branch and untracked files in the repository.
   </details>

---