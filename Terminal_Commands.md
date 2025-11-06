### Git Terminal Commands


| Command | Description |
| :--- | :---: |
| `git <command> -h` | Displays help information for the `git <command>` and all its options. |
| `git status` | Shows the current status of the repository. Useful for checking which changes have been staged, which haven't, and which files aren't being tracked by Git. |
| `git log` | Displays a log of all commits in the current branch, showing commit hashes, authors, dates, and messages. |
| `git add <file>` | Stages the specified file, preparing it to be committed. You can also use `git add .` to stage all changes in the current directory. |
| `git commit -m "message"` | Commits the staged changes to the repository with a descriptive message. |
| `git commit --amend -m "message"` | Replaces the most recent commit with a new commit, allowing you to modify the commit message or add additional staged changes. Note: This rewrites history and changes the commit hash. |
| `git commit` | When run without a message, opens the default text editor to write a commit message for the staged changes. |

