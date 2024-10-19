Basic Git Commands
Initialize a Repository

git init
Initialize a new Git repository in the current directory.

Clone a Repository

git clone <repository_url>
Clone an existing repository from a remote server to your local machine.

Check the Status

git status
Show the working tree status (modified, staged files, etc.).

Stage Files

git add <file_name>
git add .
Stage specific files or all changes for the next commit.

Commit Changes

git commit -m "Your commit message"
Record the staged changes with a descriptive message.

View the Commit History

git log
Display the commit history in the repository.

Show Differences Between Commits/Files

git diff
Show the changes between your working directory and the staging area.

Branching and Merging
Create a New Branch

git checkout -b <branch_name>
Create and switch to a new branch.

Switch to Another Branch

git checkout <branch_name>
Switch to an existing branch.

List All Branches

git branch
List all the local branches.

Merge a Branch

git merge <branch_name>
Merge changes from the specified branch into the current branch.

Delete a Local Branch

git branch -d <branch_name>
Delete a local branch after it’s been merged.

Working with Remote Repositories
Add a Remote Repository

git remote add origin <repository_url>
Connect your local repository to a remote server.

List Remote Repositories

git remote -v
Display the remote URLs.

Push Changes to a Remote Repository

git push origin <branch_name>
Push your local commits to the specified branch on the remote repository.

Pull Changes from a Remote Repository

git pull origin <branch_name>
Fetch and integrate changes from a remote branch to your local branch.

Fetch Changes from Remote (without merging)

git fetch origin
Download changes from the remote repository without merging them.

Undoing Changes
Unstage a File

git reset <file_name>
Remove a file from the staging area, keeping the changes in the working directory.

Discard Changes in a File

git checkout -- <file_name>
Revert a file to its last committed state.

Amend the Last Commit

git commit --amend -m "New commit message"
Edit the last commit message or include additional changes.

Revert a Commit

git revert <commit_hash>
Create a new commit that undoes the changes made by a specific commit.

Stashing Changes
Stash Uncommitted Changes

git stash
Save uncommitted changes and revert to a clean working directory.

Apply Stashed Changes

git stash apply
Re-apply the most recently stashed changes.

List Stashes

git stash list
List all stashed changes.

Viewing History and Logs
View Commit History with Changes

git log -p
Show the commit history along with the differences introduced in each commit.

Show One-Line Summary of Commits

git log --oneline
Show the commit history as a list of one-line summaries.

View the History of a File

git log -- <file_name>
Show the commit history of a specific file.

Show a Branching Graph

git log --graph --oneline --all
Display the commit history as a graph.

Tagging
Create a Tag

git tag <tag_name>
Create a lightweight tag for a specific commit.

Create an Annotated Tag

git tag -a <tag_name> -m "Tag message"
Create a tag with a message (annotated tag).

Push Tags to Remote

git push origin --tags
Push all tags to the remote repository.

Collaborating with Others
Rebase Changes

git rebase <branch_name>
Reapply commits from your current branch on top of another branch’s history.

Cherry-Pick a Commit

git cherry-pick <commit_hash>
Apply changes from a specific commit to your current branch.

Set Upstream Branch

git branch --set-upstream-to=origin/<branch_name> <branch_name>
Link the current local branch to a remote tracking branch.

Configuration
Set Global Username

git config --global user.name "Your Name"
Set your Git username for all repositories.

Set Global Email

git config --global user.email "your.email@example.com"
Set your Git email for all repositories.

Show Git Configuration

git config --list
Display the current Git configuration.

Submodules
Add a Submodule

git submodule add <repository_url>
Add another repository as a submodule in your current repository.

Update Submodules

git submodule update --remote
Fetch and update all submodules to their latest commits.

Other Useful Commands
Remove Untracked Files

git clean -f
Remove untracked files from the working directory.

View Command History

git reflog
Show a log of all actions performed on the repository.

Git Aliases
Create a Git Alias

git config --global alias.st status
Set an alias for the git status command (you can run git st instead).

Common Troubleshooting
Fix a Merge Conflict

# Edit conflicting files, then:
git add <resolved_file>
git commit
