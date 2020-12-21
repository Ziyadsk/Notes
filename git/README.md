# Git 
Git is a distributed version control system.  
Git helps you track the various stages of the development of your projects  
Git is light, fast & efficient   

## Create a git repository
**`git init`** 

## Cloning

**`git clone <REPOSITORY_NAME>**`**

## Status
`git status`

## Staging
`git add <FILENAME>`to add a specific file

`git add .`  to add all the file in the folder


## Commiting changes
**`git commit `**
* or use the shorthand method:   `git commit -m "<COMMIT_MESSAGE>`"

#### Fix the last commit message
`git commit --amend -m "<COMMIT_MESSAGE>`
> you can add files and --amend to last commit
## 
* fetch 
* pull 
* push
 
* commit 
* tag
* stash
* reset

### Restore uncommited local changes
* `git restore <FILE_NAME>` return to the last change or restore if deleted
* `restore -p <FILE_NAME> ` for specific changes in a file
  
* `git restore .` to discard all current changes in the repo
* `git restore --source <COMMIT_HASH> <FILE_NAME>` restores a single file from a specific commit
### Revert
#### undo by creating a new commit 
`git revert <COMMIT_HASH>`

### Reset
#### undo
`git reset --hard <COMMIT_HASH>`

### Log
### diff

## Branches
### delete a branch
`git branch -d <BRANCH_NAME>`