# Task Manager UI

## To clone the repo:
### Install git:
Platform Dependent:
Do check this : https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

After installation use the following command to clone the repository
> git clone https://github.com/atishekk/atishekk.github.io.git

### To access the site
Use the following URL:
> https://atishekk.github.io

## How to make changes to the repository
All the instructions are for a command line interface.

### 1.Clone the repository
First you need to clone the repository as explained above. Also do configure your personal details.
> git config user.name "<Name>"
> git config user.email "<email>"
You can use the --global flag to set these configuration changes globally

### 2.Create a separate branch.
Please don't work on the master. Create a new branch for implementing a new feature and create a pull request.
To create a new branch
> git checkout -b "<branch name>"
To list different branches and check which branch you are working on
> git branch
To select a branch
> git checkout "<branch name>"
Note : master is the name of the default branch and all the changes to the master should be done after reviewing the pull request.

### 3.Making changes
Make sure you are not on the master branch.
After making the required changes to the code save them. Now to tell git to track these changes use the following
> git add <filename>    //can list multiple files a well
To add all the files which were changed
> git add --all

Now to commit or finalise these changes
> git commit -m "message"
Make the messages meaningful try and summarise the changes made.
You can also use the following to add and commit the changes in one step
> git commit -am "message"

### 4.Making these changes available to others
After testing your code throughly push these changes to the servers
> git push origin <branch name>
If it is the first time you are pushing changes for a newly created branch use
> git push --set-upstream origin <branch name>
Now create a new pull request on the GitHub website to add your code to the master branch. Your code will be reviewed and discussed and if accepted will be merged.

### Other helpful commands
To get the status of the repository
> git status
To get the list of commits
> git log
Note : Each commit is given a hash value to uniquely identify it

To see the difference betweeen two commits
> git diff <old commit hash>..<new commit hash>

To back to a previous change/commit
> git reset --hard <commit hash>

To get updated code from the servers on your local system
> git pull
