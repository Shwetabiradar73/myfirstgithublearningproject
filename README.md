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
1.mkdir yourprojectname   - it creates a new directory
2.cd yourprojectname    - current working directory

->git init -- to check we are in correct folder we can initialize using this command

      stage a file/files
1.git add filename  - it adds one file
2.git add --all/git add -A 

1.Staged the wrong file? Use git restore --staged <file> to unstage it.
2.Forgot to stage a file? Just run git add <file> again before you commit.
3.Not sure what's staged? Run git status to see what will be committed.

->git reset HEAD index.html/git restore --staged index.html  - used to unstage a file

		Commiting
1.git commit -m "message" - Commit staged changes with a message
2.git commit -a -m "message" - Commit all tracked changes (skip staging)
3.git log - See commit history

      Forgot to stage a file?
1.If you run git commit -m "message" but forgot to git add a file, just add it and commit again. Or use git commit --amend to add it to your last commit.
2.Typo in your commit message?
3.Use git commit --amend -m "Corrected message" to fix the last commit message.
4.Accidentally committed the wrong files?
5.You can use git reset --soft HEAD~1 to undo the last commit and keep your changes staged.

      To push into github repository
1.git remote add origin https://github.com/shwetabiradar/myfirstgithublearningproject.git
2.git push -u origin master
3.git remote -v - for tracking

