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

- git status # check files, check history
- git add -u :/ # adds all modified file changes to the stage; analgus to confirm the changes
- git add * :/ # adds modified and any new files (that's not gitignore'ed) to the stage
- git commit -m 'your commit comment'   # equivalent to save the file
- git commit -am 'your commit comment'   # perform add and commit 
- git push origin master # or just git push origin master
- git log # show the history, who, when and what 
- git reflog # random hash for each commit
- git show # show last command
- gitk # gui for history, id etc of commits sumbitted
- git checkout [filename] # convert back to original file.
- git reset --hard [commit id]  # set HEAD to the old commit idenified by id  

#### _Tips_   
hit q to exit \\
add -h flag to get help: e.g. git show -h


## How commit works
The HEAD is the first change we commited followed by others with commit comments. Each commit has it own id and arranged in order. 

![](/post/2018-12-02-git-basics_files/Screen Shot 2018-12-01 at 9.23.33 PM.png)

I am adding non sense here.