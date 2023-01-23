# GitPrac1
Git Practical 1 

- Create a demo java application.

- Commit application to GitHub account

- Create a branch and make changes and commit changes in the branch

- Create a pull request and merge it with the master branch


git init
  Initialized empty Git repository in /home/nimit/IdeaProjects/Demo/.git/

touch .gitignore
git status
  On branch master

  No commits yet

  Untracked files:
    (use "git add <file>..." to include in what will be committed)
	  Demo.iml
	  out/
	  src/
  
git add .
git status
  On branch master
  
  No commits yet

  Changes to be committed:
    (use "git rm --cached <file>..." to unstage)
	    new file:   Demo.iml
	    new file:   out/production/Demo/Main.class
	    new file:   src/Main.java

git commit -m "First Commit -App Addded"
  [master (root-commit) 533109d] First Commit -App Addded
  3 files changed, 16 insertions(+)
  create mode 100644 Demo.iml
  create mode 100644 out/production/Demo/Main.class
  create mode 100644 src/Main.java
  
git remote add origin git@github.com:MN-Simform/GitPrac1.git
git remote -v
  origin	git@github.com:MN-Simform/GitPrac1.git (fetch)
  origin	git@github.com:MN-Simform/GitPrac1.git (push)
  
git push -u origin master
  Enumerating objects: 9, done.
  Counting objects: 100% (9/9), done.
  Delta compression using up to 4 threads
  Compressing objects: 100% (5/5), done.
  Writing objects: 100% (9/9), 1.29 KiB | 1.29 MiB/s, done.
  Total 9 (delta 0), reused 0 (delta 0), pack-reused 0
  To github.com:MN-Simform/GitPrac1.git
    * [new branch]      master -> master
  Branch 'master' set up to track remote branch 'master' from 'origin'.
  
git checkout -b dev
  Switched to a new branch 'dev'
  
git branch 
  * dev
    master
  
git status
  On branch dev
  Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
	    modified:   out/production/Demo/Main.class
	    modified:   src/Main.java
  
git add .
git status
  On branch dev
  Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
	    modified:   out/production/Demo/Main.class
	    modified:   src/Main.java

  
git commit -m "Dev Branch -Add Pyramid"
  [dev a71a7df] Dev Branch -Add Pyramid
    2 files changed, 9 insertions(+)
  
git push origin dev
  Enumerating objects: 15, done.
  Counting objects: 100% (15/15), done.
  Delta compression using up to 4 threads
  Compressing objects: 100% (4/4), done.
  Writing objects: 100% (8/8), 726 bytes | 726.00 KiB/s, done.
  Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
