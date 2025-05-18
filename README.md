🔧 GIT Configuration

ls – Lists files in your current directory (not a Git-specific command).

git --version – Check your installed Git version.

git config --global core.editor "code --wait" – Set VS Code as the default editor.

git config --global user.name "Your Name" – Set your Git username.

git config --global user.email "your@email.com" – Set your Git email.

git config --list – Show all configured Git settings.

git config user.name or git config user.email – View the configured name/email.

git config --global --unset core.editor – Unset a specific config setting.

Git config levels:

System: git config --system user.name "System Name"

Global: git config --global user.name "Your Name"

Local: git config --local user.name "Project-Specific Name" or omit --local inside a repo.

📁 Creating & Initializing a Git Repository

mkdir yourprojectname – Create a new project folder.

cd yourprojectname – Navigate into your project folder.

git init – Initialize a new Git repository in the folder.

📥 Staging Files

git add filename – Stage a specific file.

git add --all or git add -A – Stage all changes (new, modified, deleted files).

git status – Check which files are staged or not.

Helpful Tips:

Wrong file staged? → git restore --staged <file>

Forgot to stage? → Just run git add <file>

Unstage file: git reset HEAD <file> or git restore --staged <file>

✅ Committing Changes

git commit -m "message" – Commit staged changes with a message.

git commit -a -m "message" – Commit tracked changes directly (skip staging).

git log – Show commit history.

Fixes:

Forgot a file? → Add it and run git commit --amend.

Typo in message? → git commit --amend -m "Corrected message"

Undo last commit (keep changes): git reset --soft HEAD~1

🚀 Pushing to GitHub
git remote add origin https://github.com/username/projectname.git – Link to GitHub repo.

git push -u origin master – Push your code and set upstream branch.

git remote -v – View the remote URLs Git is tracking.
