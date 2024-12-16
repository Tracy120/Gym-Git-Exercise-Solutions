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
