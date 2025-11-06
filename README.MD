# **Introduction to Git(this is a test)**

### **Table of Contents**
1. - #### [Setting Up a New Git Repository](#setting-up-a-new-git-repository)
2. - #### [Various Git/Github Workflow](#various-gitgihub-workflow)
      - [*If you are using Microsoft Visual Studio Code*](#microsoft-visual-studio-code)
      - [Useful Git Commands](#useful-git-commands)

#### **Setting Up a New Git Repository**
1. **Navigate to Your Project Directory**  
   Open CMD and use the command `cd <directory>`. Alternatively, open a command prompt (cmd) in the project folder.

2. **Initialize a New Git Repository**  
   Use the command `git init`. The command initializes a new Git repository in your current directory.

3. **Stage a README.md File**  
   Add the file to the staging area using the command:
   ```bash
   git add README.md
   ```

4. **Commit Changes**  
   Use the command:
   ```bash
   git commit -m "Your commit message here"
   ```
   Replace "Your commit message here" with a description.

5. **Check Repository Status**  
   Check the status of your repository with:
   ```bash
   git status
   ```
   You should see `README.md` listed as modified or a new file.

6. **Stage All Changes**  
   Run:
   ```bash
   git add -A
   ```
   Alternatively, run `git status` again to see the changes. If `README.md` is untouched, you should see the output:
   ```
   On branch master
   Changes to be committed:
   (use "git restore --staged <file>..." to unstage)
           modified:   README.md
   ```

7. **Create a New Repository on GitHub**  
   Navigate to [github.com](https://github.com) and create a new empty repository. Do not initialize it with a README.md, .gitignore, or license. Copy the repository URL.

8. Back in your terminal, add the remote repository URL using the command:
   ```bash
   git remote add origin <URL>
   ```
   Replace `<URL>` with the copied repository URL.

9. **Rename Your Branch**  
   Use:
   ```bash
   git branch -M main
   git push -u origin main
   ```

10. **Create a .gitignore File**  
   Create a .gitignore file and include necessary files and folders to be ignored by git. Alternatively, you can use a template from [GitHub's gitignore repository](https://github.com/github/gitignore) or generate one [at Toptal's gitignore generator](https://www.toptal.com/developers/gitignore).


11. **Stage and Commit the .gitignore File**  
   Stage and commit the .gitignore file using:
   ```bash
   git add .gitignore
   git commit -m "Add .gitignore file"
   git push --all
   ```
12. **Merge branches.**
   ```bash
   git checkout target-branch
   git merge source-branch
   git add .
   git commit -m "merged old branch with new"
   git push origin target-branch
   ```

# Various Git/Github Workflow

## Microsoft Visual Studio Code
   If you are using Visual Studio Code, you can install the [GitLens extension](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) to help with git commands and visualizations. This will let you see changes, commits, branches, and more directly in the editor.
   
   There is also a [markdown preview extension](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced "Markdown Preview Enhanced") that will let you preview markdown files in vscode.

## Useful Git Commands
the `<link to file>` provides a couple of useful git commands for various tasks.