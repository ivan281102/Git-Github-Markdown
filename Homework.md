# Basic Commands

Here are some commands that we can use to be faster when we are working

## Directories

`mkdir {Directory Name}` mkdir is the abreviation for make directory, to use it correctly we only need to type this followed by the directory name.

`rmdir {Directory Name}` rmdir is the abrevation for remove directory, to use it correctly we only need to type this followed by the directory name.

## Navigate

`cd` We can use cd followed by the route we want to go to move throghout the directories.

## Compare 

`cmp` It is used to compare the two files byte by byte and helps you to find out whether the two files are identical or not.

## Find files, folders and inside files

`find {Route} {Name or extension}`This is kind of difficult to explain so we have this example: find /home/example-username/ -filename_example

## Create and edit files

`nano` There are a lot of ways to create and edit a file but here we have nano because as my way to see, is the easiest, just type nano followed by the name of the file we want to create or edit.

## Get the state of the computer 

`lscpu`At least in Linux, which is the operating system I use, this command is useful to see the state of the computer.

# The git / github

Here are some of the most important commands we can use in git

## The initial configuration

We need to set up our environment in which we are going to work. For this, git provides us some cheats to set default values. Like this ones:

`$ git config --global user.name "Your name"` This set us the name that will be attached tp our commits and tags.

`$ git config --global user.email "Your email"` It is like the previous one, just that is our email, not our name (It shows in commits and tags).

## Starting a project from zero 

We have to start our project, for this, git gives us these tools:

`$ git init {project name}` This will create a local repository inside of a directory created locally as well.

`$ git clone {project url}` This comman will download a project from a remote repository.

## Basic workflow commands to stage and commit

If we start a project, we need to use some commands.

`$ git status` This is probably the command that we will use most when we are working, because, this command displays the status of thw working directory, showing us created, deleted or modified files

`$ git add {file}` This command will be used for staging your files, ready to commit them.

`$ git diff {file}` It shows changes between our working directory and the staging area.

`$ git diff --staged {file}` It shows changes between the staging area and the local repository.

`$ git reset {file}`This cheat will make our repository return to a previous known state.

`$ git commit` Creates a new commit of the changes that are in the staging area. 

`$ git rm {file}` Probably, sometimes you will need to undo things or to add something to your staging area and this command would be helpful for some of this cases, will remove the file from the working directory and staging area.

`$ git stash`  I think this cheat was not seen in class, but in my experience as a git user, I think is very useful, it saves the current changes of the working directory into a stash so we can use them later.

`$ git stash pop` Applies the stored changes in the stash into the working directory again.

##Branches

To modify our project or work, without affecting in other changes or features git provides us this commands.

`$ git branch {-a}` Shows a listing of all local branches.

`$ git checkout {-b}{branch_name}` Switches our working directory to the specified branch, the [-b] creates a new branch if it does not exist.

`$ git merge {from name}` It merges or joins two branches, the [from name] to the current branch.

`$ git branch -d {name}` When we merge a branch to another, the branch that has been merged, is now "useless", so we can remove thibranch if is already merged in any other.

##Gitflow

To see, what we are doing in the project, who commited or did changes, git has this command.

`$ git log {-n count}` Lists all the commits specified, for this, just replace n for the limit wanted.
