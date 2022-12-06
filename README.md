Git command


1) Create New Branch
* git checkout -b nazmul


2) Git Merge [rebase same purpose serve]
* git merge nazmul


3) Git Rebase
* git rebase nazmul


4) Git Fetch/ Pull
* git fetch
* git fetch nazmul [branch name]
* git fetch - -all


5) Git Reset
* git reset - -hard 82c38653cabbe28405b4a1b1a0f15dcdff7ac8fd [commit_id]


6) Git Clone
* git clone url


7) Git Branch Rename
* git branch [check current active branch]
* git branch -m nazmulh [this command make nazmul branch as nazmulh]


8) Git Branch Delete
* git branch -D test [can’t delete active branch so need to checkout from test branch]


9) Git Stash
* if you just need to checkout in a different branch and you are not ready to commit for the changes you currently have.
* or If you discover that you are in a wrong branch and your changes need to be in different branch.
* Creating a stash save uncommitted changes. Checkout your current branch and git stash pop to save the stash in your current/own branch.
* git stash
then checkout in your current branch
* git stash pop
* git add .
* git commit -m "commented code removed"
* git push


10) Git Cherry pick


* Bring in changes from a specific commit [from any branch by commit id]
* If someone fixed a bug that you have in your branch and you want to bring just in one commit but not the whole branch.
* You can choose one commit or multiple commit to brought into your branch[]


0.1) Checkout this branch find all the commit [git log] 
0.2) then checkout my branch
* git cherry-pick 787887989[commit_id]
* git cherry-pick 787887989 98888 5657687 [for multiple commit_id]


11) Git diff
* Git diff show the changes what i write after my last commit.
* git diff




#New git branch create & upload code from another branch

1) git branch nazmul[code exist in master branch]
2) git checkout nazmul
3) git pull origin master
4) git push

# Easy way git keep update
1) Commit in my branch [nazmul branch]
2) git checkout dev [dev branch a shift holam]
3) git pull [dev branch e update thakle namalam]
4) git merge nazmul [merge nazmul with dev, now both branch is uptodate]
5) git push

#Freash file push in a git project

1) clone existing project
2) checkout the branch you want to take your code
3) copy .init, git ignore and gitattributes and paste in the new code what you want to push at git repo
4) git fetch --all
5) git commit
6) git push


# gitrules

Pull code from any branch
<!--amar branch e theke rezaul branch er update code amar branch e namano  -->
<!--amar branch e thekei  -->
1) git pull origin rezaul
2) git push

Je kono commit e ferot jao a

git reset --hard 82c38653cabbe28405b4a1b1a0f15dcdff7ac8fd  [commit_id]

1)Git notun branch er update check kore, notun branch e Nazmul branch marge kora

1.1) git checkout dev (dev branch e jaowa)
1.2) git pull ( dev branch e update kono file thakle namabe)
1.3) git merge nazmul (amar code gulo dev branch er locally niea ashbe)
1.4) git push(amar code gulo live e gelo)


#Adding an existing project to GitHub using the command line

Simple steps to add existing project to Github.

1. Create a new repository on GitHub.
In Terminal, change the current working directory to your local project.

##2. Initialize the local directory as a Git repository.

git init
Add the files in your new local repository. This stages them for the first commit.

git add .
or:

git add --all
Commit the files that you've staged in your local repository.

git commit -m 'First commit'
Copy remote repository URL field from your GitHub repository, in the right sidebar, copy the remote repository URL.

In Terminal, add the URL for the remote repository where your local repostory will be pushed.

git remote add origin <remote repository URL>
Sets the new remote:

git remote -v
Push the changes in your local repository to GitHub.

git push origin master
Pushes the changes in your local repository up to the remote repository you specified as the origin

//////////////////////////////////////////
  
1) git rm -r --cached .
2) git add .
3) git commit -m ".gitignore is now working"

git clone url --single-branch --(branch name)branch development 
git clone https://github.com/bKash-developer/pgw-merchant-backend-php --single-branch --branch development 

  
// Work with git branch
  
git checkout -b branch1  // git create new branch name branch1
  
git branch --list // check all git branch 
  
git checkout branch1 // go to branch name branch1

git push --set-upstream origin branch1 // branch1 e upload kora [from last checkout branch]
  
#laravel project clone

1) Clone your project : git clone url
2) Copy .env.example file to .env on the root folder. 
3) Run php artisan key:generate
4) composer install & composer update
4) Run php artisan migrate
5) Run php artisan serve
Go to localhost:8000


vue reprojectory run

Clone the repository with git clone
Copy .env.example file to .env and edit database credentials there
Run composer install
Run php artisan key:generate
Run php artisan migrate
Run npm install
Run npm run dev


