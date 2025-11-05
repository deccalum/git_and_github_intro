# Introduction to Git


    1. First navigate to your project directory with the "cd <directory>" command or open a cmd instance in the project folder.

    2. Use the command "git init". The command initializes a new Git repository in your current directory.

    3. Add this file (README.md) to the staging area using the command "git add README.md".

    4. Use the command "git commit -m "comment"" to commit changes. Replace "comment".

    5. Check status of your repository with "git status". README.md should be listed as modified or new file.

    6. Run "git add -A" to stage all changes in the repository. Alternatively run "git status" again to see the changes, if the README.md is untouched you should see the output: 
    On branch master
    Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
            modified:   README.md

    7. Navigate to github.com and create a new empty repository. Do not initialize with README.md, .gitignore or license. Copy the repository URL.

    8. Back in your terminal, add the remote repository URL using the command "git remote add origin <URL>". Replace "<URL>" with the copied repository URL.

    9. Use "git branch -M main" followed by "git push -u origin main".

    10. Create a .gitignore file and include necessary files and folders to be ignored by git. Alternatively, you can use a template from [here](https://github.com/github/gitignore) or generate one [at](https://www.toptal.com/developers/gitignore).