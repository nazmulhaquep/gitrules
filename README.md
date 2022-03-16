# Easy way git keep update
1) Commit in my branch [nazmul branch]
2) git checkout dev [dev branch a shift holam]
3) git pull [dev branch e update thakle namalam]
4) git merge nazmul [merge nazmul with dev, now both branch is uptodate]


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

git push --set-upstream origin branch1 // branch1 e upload kora 
  
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


