# git-expt-4
My Git Experiment 4 repository






























1)
git init
git status
git add my_file.txt
git status
git commit -m "Add my first file"
git commit -m "Add a new file called my_file.txt"

2)
cd gitexpmt
git branch
git checkout -b feature-branch
git add .
git commit -m "Add feature branch file"
git checkout master
git merge feature-branch

3)
cd gitexpmt
git status
git stash save "Experiment 3 changes"
git checkout feature-branch
git stash apply

4)
cd ~/gitexpmt
pwd
git clone https://github.com/NidhishIB08/Git-Ext-4.git
ls
cd Git-Ext-4
pwd
ls
git remote -v
git status

5)
cd ~/gitexpmt/Git-Ext-4
pwd
git status
git checkout -b exp5-local
echo Local changes for Experiment 5 > local.txt
git add .
git commit -m "Add local changes for experiment 5"
git checkout exp5-local
git fetch origin
git rebase origin/main
git push origin exp5-local
git status
git log --oneline --graph --all

6)
cd ~/gitexpmt/Git-Ext-4
git checkout feature-branch
git cherry-pick 4c1f154
git checkout master
git reset --hard 1e67298
git merge feature-branch -m "Merging feature branch into master"
git branch
git log --oneline --graph --all
git status
git reset --hard 1e67298
git merge --no-ff feature-branch -m "Merging feature branch into master"
git log --oneline --graph --all
git status








1)
git init
git status
echo "Hello Git" > my_file.txt
git add my_file.txt
git commit -m "Add my first file"

2)
git branch
git checkout -b feature-branch
echo "Feature changes" > feature.txt
git add .
git commit -m "Add feature"
git checkout master
git merge feature-branch

3)
git status
git stash
git checkout master
git stash apply

4)
cd ~/gitexpmt
git clone https://github.com/NidhishIB08/Git-Ext-4.git
cd Git-Ext-4
pwd
ls
git remote -v
git status

5)
git checkout -b exp5-local
git add .
git commit -m "Add local changes"
git fetch origin
git rebase origin/main
git push origin exp5-local

6)
git checkout -b feature-branch
git add .
git commit -m "Add feature changes"
git checkout master
git merge --no-ff feature-branch -m "Merging feature branch into master"
git branch
git log --oneline --graph --all
git status