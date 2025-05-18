--------------Git commands------------

   GIT Congigurations
1.ls - to add files to your folders
2.git --version - to check the version of you git
3.git config --global core.editor "code --wait"  - settings to your wish editor vs code/notepad,android studio etc
4.git config --global user.name - "your name" -- setting your name
5.git config --global user.email - "your email" -- setting your mail
6.git config --list - to get the list of all you settings or changes
7.git config user.name/user.email - checking your name/email
8.--unset - used to remove a setting eg.git config --global --unset code.editor
9.System (all users): git config --system  eg.git config --system user.name "System Name"
  Global (current user): git config --global eg.git config --global user.name "Project Name"
  Local (current repo): git config --local  eg.git config user.name "Project Name"


    Creating Git Folder
mkdir yourprojectname   - it creates a new directory
cd yourprojectname    - current working directory

git init -- to check we are in correct folder we can initialize using this command

      stage a file/files
1.git add filename  - it adds one file
2.git add --all/git add -A 

Staged the wrong file? Use git restore --staged <file> to unstage it.
Forgot to stage a file? Just run git add <file> again before you commit.
Not sure what's staged? Run git status to see what will be committed.

git reset HEAD index.html/git restore --staged index.html  - used to unstage a file

		Commiting
git commit -m "message" - Commit staged changes with a message
git commit -a -m "message" - Commit all tracked changes (skip staging)
git log - See commit history

      Forgot to stage a file?
If you run git commit -m "message" but forgot to git add a file, just add it and commit again. Or use git commit --amend to add it to your last commit.
Typo in your commit message?
Use git commit --amend -m "Corrected message" to fix the last commit message.
Accidentally committed the wrong files?
You can use git reset --soft HEAD~1 to undo the last commit and keep your changes staged.

      To push into github repository
git remote add origin https://github.com/shwetabiradar/myfirstgithublearningproject.git
git push -u origin master
git remote -v - for tracking

