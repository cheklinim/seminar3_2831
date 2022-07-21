# **Instructions for working with the version control system**

__GIT__ *is software for tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software development.*

![logo](git_logo.png)

## Repository initialization

    git init 

*in order to do the magic of the git in the folder.*
  
    git add  < file name.file extension > 

*to track the desired file and do it after changes have been made.*

## Checking the status of a repository

    git status 

*to check file status.*

    git status -s 
    
*short status.*

## Adding versioning

 *to add new versions: make changes; save file; do:* 

     git add  <file name.file extension> ---> 
     git commit -m "text"

*or*

    git commit -a -m "text"

## Committing the change

     git commit -m "text" 

*to describe the changes.*

## View commit history

    git log : 

*to see the history of changes.*

    git log --oneline  

*short version.*

    git log --stat 

*more detail.*

    git log --graph 

*see the progress of the branches*

   
    git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all

*full compack understandable list of changes*

## Switching between versions

    git checkout <the first four simbols of log> 

*look at the status in the version < log >.*

    git checkout master 

*back in the main status.*

    git diff

*to see the difference between the current version and the latest commited version*

    git diff <log_a> <log_b>

*to compare versions differences*

## Branching in GIT

*Allows you to develop different versions of the source in parallel with the possibility of merging them*

    git branch < name >

*to add new branch*

    git branch

*to check which branch you are on*

    git checkout < branch name >

*to switch on branch*

    git checkout master

*return to the main branch*

    git branch -d < branch name >

*to delete unnecessary branch*

    git branch -D < branch name >

*force deletion of a branch from which changes have not been merged*

## Merging in GIT

    git merge < branch name >

*to merge the shown branch with the current one*

## Working with remote repositories

__*remote repository is the cloud storage of your files. allows you to work with projects from anywhere in the world where there is Internet*__

    git remote add origin <link> ---->
    git branch -M <name of main branch(mostly "master")> ---->
    git push -u origin <name of main branch(mostly "master")

*to make friends with the local and remote repository*
    git pull

*to drag the changes from the remote repository and merge them with your version on the PC*

    git push

*to send the changes from the your PC and merge them with remote repository virsion*

# Fork

__*for selecting a clone operation performed on someone else's server copy of the project repository and then creating a clone or copy of it.*__

*on gitub.com or or other suitable site click "Fork" on the repository you are interested in*

---> on markdown

    git clone <link>

*for selecting an existing repository and then creating a clone or copy of it.*

--->

    cd <folder>

---
    
    git push

*to puch changes to main branch*

    git  push --set-upstream origin <branch name>

*to puch changes to your branch*

# Pull request

*on github in the tab with the gentle repository after the changes have been made, click on the compare & pull request to send the proposed changes to the owner of the repository*

## Оther useful commands

    clear 

*to clear the terminal.*

    mv test_main_file.c test_main.c ---> 
    git add <new file name> ---> 
    git commit -m "rename file" ---> 
    git rm <old name>

*to rename file*

------------------------

# Instructions for working with Markdown

## Text formatting

to italicize text, it must be framed in (*) or (_).
 for example: *like this* or _like this_

to semi-bold text, it must be framed in (**) or (__).
 for example: **like this**, or __like this__

alternative methods are needed in order to combine them.
 for example : _**like this**_

## Lists 
 
 to add unnumbered  lists, items need to be highlighted (*) or (+). 
 for example:
 * el_1
 * el_2
 * el_3
 + el_4

 to add numbered  lists, items need to be numbered . 
 for example:
 1. el_1
 2. el_2
 3. el_3

## Work with images

 to insert an image write this:
 ![text](image.format) 
 
 --->

 commite changeds

 --->

 create new file with name: .gitignore

 --->

 add image.format in .gitignore

 --->

add and commit .gitignore

## Links

[Link text Here](https://gb.ru/)

