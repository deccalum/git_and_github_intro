# Introduction to Git


## First navigate to your project directory with the "cd <directory>" command or open a cmd instance in the project folder.

## Use the command "git init". The command initializes a new Git repository in your current directory.

## Add this file (README.md) to the staging area using the command "git add README.md".

## Use the command "git commit -m "comment"" to commit changes. Replace "comment".

## Check status of your repository with "git status". README.md should be listed as modified or new file.

## Run "git add -A" to stage all changes in the repository. Alternatively run "git status" again to see the changes, if the README.md is untouched you should see the output: 
    On branch master
    Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
            modified:   README.md

## Navigate to github.com and create a new empty repository. Do not initialize with README.md, .gitignore or license. Copy the repository URL.

## Back in your terminal, add the remote repository URL using the command "git remote add origin <URL>". Replace "<URL>" with the copied repository URL.

## Push your changes to the remote repository using the command "git push -u origin master".