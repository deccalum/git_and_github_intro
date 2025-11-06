# **Introduction to Git**

## **Table of Contents**
 - ###### [Setting Up a New Git Repository](#setting-up-a-new-git-repository)
 - ###### [Various Git & GitHub Workflow](#various-git-&-github-workflow)
      - [*If you are using Microsoft Visual Studio Code*](#microsoft-visual-studio-code)
      - [*Markdown Cheat Sheet*](#markdown-cheat-sheet)
      - [*Useful Git Commands*](#useful-git-commands)




## **Setting Up a New Git Repository**
1. **Navigate to Your Project Directory**  
   - Windows: Open CMD and run the command `cd <directory>`. Alternatively, open a command prompt in the project folder.
   - Mac/Linux: Open Terminal and use the command `cd <directory>`.

2. **Initialize a New Git Repository**  
   Run the command `git init`. The command initializes a new Git repository in your current directory.

3. **Stage a README.md File**  
   Add the file to the staging area by running the command:
   ```bash
   git add README.md
   ```

4. **Commit Changes**  
   Run the command:
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
   Go to [GitHub](https://github.com) and create a new empty repository. Do not initialize it with a README.md, .gitignore, or license. Copy the repository URL.

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

10. **Create** `.gitignore`  
   Create a `.gitignore` file and include necessary files and folders to be ignored by git. Alternatively, you can use a template from [GitHub's gitignore repository](https://github.com/github/gitignore) or generate one [at Toptal's gitignore generator](https://www.toptal.com/developers/gitignore).


11. **Commit** `.gitignore` 
   Stage and commit the `.gitignore` file using:
   ```bash
   git add .gitignore
   git commit -m "Added .gitignore file"
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
13. **When making changes to files...**
   ```bash
   git status
   git add <file>
   git commit -m "describe changes made"
   git push
   ```


## Various Git & GitHub Workflow

##### Microsoft Visual Studio Code
   If you are using Visual Studio Code, you can install the [GitLens extension](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) to help with git commands and visualizations. This will let you see changes, commits, branches, and more directly in the editor.
   
   There is also a [markdown preview extension](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced "Markdown Preview Enhanced") that will let you preview markdown files in vscode.

##### Markdown Cheat Sheet
[Markdown Cheat Sheet](https://markdowncheatsheet.com/reference) Provides a comprehensive in-depth guide to markdown syntax, including extended features like tables, footnotes, and task lists.

##### Useful Git Commands
The [Terminal Commands](./Terminal_Commands.md) file provides a couple of useful git commands for various tasks.