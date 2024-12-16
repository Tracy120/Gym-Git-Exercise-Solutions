
# EXERCISE 1
```bash
pc@DESKTOP-OTTEP0S MINGW64 ~
$ git config --global user.name "Tracy120"

pc@DESKTOP-OTTEP0S MINGW64 ~
$ git config --global user.email "uwasetracy@120"

pc@DESKTOP-OTTEP0S MINGW64 ~
$ cd Documents

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents
$ mkdir myproject
mkdir: cannot create directory ‘myproject’: File exists

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents
$ mkdir "myproject"
mkdir: cannot create directory ‘myproject’: File exists

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents
$ cd myproject

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject
$ git init
Initialized empty Git repository in C:/Users/pc/Documents/myproject/.git/

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ ls index.html
index.html

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git add index.html
warning: in the working copy of 'index.html', CRLF will be replaced by LF the next time Git touches it

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git add "index.html"

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html


pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$
pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git commit -m "okay"
[master (root-commit) 973e3ea] okay
 1 file changed, 12 insertions(+)
 create mode 100644 index.html

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git status --short
?? README.md

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git commit -m "committed"
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$
pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git branch
* master

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (master)
$ git branch -m master main

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (main)
$
pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (main)
$ git add .
git commit -m "Initial commit"
warning: in the working copy of 'README.md', CRLF will be replaced by LF the next time Git touches it
[main 312799a] Initial commit
 1 file changed, 9 insertions(+)

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (main)
$ git remote add origin https://github.com/Tracy120/Gym-Git-Exercise-Solutions.git

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (main)
$ git push -u origin main
fatal: unable to access 'https://github.com/Tracy120/Gym-Git-Exercise-Solutions.git/': Could not resolve host: github.com

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (main)
$ ^C

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (main)
$ git push -u origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (9/9), 1.42 KiB | 363.00 KiB/s, done.
Total 9 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Tracy120/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (dev)
$ git branch
* dev
  main

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (dev)
$ git checkout dev
git checkout -b test
Already on 'dev'
M       README.md
Switched to a new branch 'test'

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (test)
$ git checkout dev
git merge test
Switched to branch 'dev'
M       README.md
Already up to date.

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (dev)
$ git branch -d test
Deleted branch test (was 312799a).

pc@DESKTOP-OTTEP0S MINGW64 ~/Documents/myproject (dev)
$ git push origin main


