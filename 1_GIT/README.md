# GIT

## Installation

**Linux**

apt install git -y

**Mac OS**

`brew install git`
OR
`xcode-select --install`

**Windows**

Download and install from [this link](https://gitforwindows.org/)

OR use **SWL**

## Basics

### Clone a repository

`git clone [remoterepository]`

eg. `git clone https://github.com/djimondev/CESI-Nancy-MAALSI-Infra-si`

### Add files into our commit

`git add [filepath]`

eg.

`git add README.md` <- add a file

`git add 0_BONUSES\.` <- add every files in a folder

`git add 0_BONUSES\markdown.md` <- add a specific file within a folder

`git add .` <- Add every files in current folder

`git add -A` <- same :)

### Create your commit

`git commit -m "Added a command in linux doc et going ahead in git"`

### Push your commit

`git push`

### Retrieve code

`git pull`

### Check status

`git status`

## Branches

### Show branches

`git branch -a`

### Checkout an existing branch

`git checkout [name_of_the_branch]`

Eg.
`git checkout main`

### Create a branch

`git checkout -b [name_of_the_branch]`

Eg.
`git checkout -b develop`

## Advanced

### See my current modifications

`git diff`

### put my modifications in a buffer

`git stash`

### retrieve from the buffer

`git stash pop`
