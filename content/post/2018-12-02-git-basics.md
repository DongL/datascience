---
title: Git basics
author: Dong Liang
date: '2018-12-02'
slug: git-basics
categories: []
tags: []
---


## Online tutorial for Git 
[![How to use Git](http://img.youtube.com/vi/DQUcmNO4diQ/0.jpg)](https://www.youtube.com/watch?v=DQUcmNO4diQ&list=PLeAngWE7pYE5lXCjbmg0C1hM-w0kPIFZA "How to use Git")


## Some basic command

### Add-commit-push 
- git add -u :/ # adds all modified file changes to the stage; analgus to confirm the changes
- git add * :/ # adds modified and any new files (that's not gitignore'ed) to the stage
- git commit -m 'your commit comment'   # equivalent to save the file
- git commit -am 'your commit comment'   # perform add and commit 
- git push origin master # or just git push origin master

### Check history
- git status # consistency status with branch master, change not staged for commit, untracked file.
- git log # show the history, who, when and what 
- git reflog # random hash for each commit
- git show # show last command
- gitk # gui for history, id etc of commits sumbitted

### Revoke
- git checkout [filename] # convert back to original file.
- git reset --hard [commit id]  # set HEAD to the old commit idenified by id  

### Ignore



### _Tips_   
hit q to exit \\
add -h flag to get help: e.g. git show -h


## The add - commit - push workflow
`git add` : modified \\
`git commit` : saved



## How commit works
The HEAD is the first change we commited followed by others with commit comments. Each commit has it own id and arranged in order. 

![](/post/2018-12-02-git-basics_files/Screen Shot 2018-12-01 at 9.23.33 PM.png)

## How HEAD works
HEAD is pointing to the changes just committed by default. We can use `git reset --hard [commit id]`, to force HEAD jump back to old commits. In this case, `git push` command will get rejected because the tip of the current branch is not in agreement. Use `git push --force` to overide the one on the remote server. 

```
git reflog
```

![](/post/2018-12-02-git-basics_files/Screen Shot 2018-12-01 at 10.18.01 PM.png)


