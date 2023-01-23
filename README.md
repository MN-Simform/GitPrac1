# GitPrac1
Git Practical 1 

- Create a demo java application.

- Commit application to GitHub account

- Create a branch and make changes and commit changes in the branch

- Create a pull request and merge it with the master branch


git init

touch .gitignore
  
git add .

git status

git commit -m "First Commit -App Addded"
  
git remote add origin git@github.com:MN-Simform/GitPrac1.git

git remote -v
  
git push -u origin master

git checkout -b dev
  
git branch 
  
git status

git add .

git status
  
git commit -m "Dev Branch -Add Pyramid"
  
git push origin dev
