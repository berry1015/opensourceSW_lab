# About *'Git'* 

## ✨3 states in Git
![image](https://github.com/user-attachments/assets/2a1484be-cf20-4ca0-88bf-173935e776a3)  
<br>

## ✨Git config: First-time setup
Git configurations are stored in 3 levels:
> 1) System level        : --system option. Affects all uses and repositories on system(administrative)  
       file> /etc/gitconfig
> 2) Global (user) level : --global option. Affects all repositories of a current user  
       file> ~/.config/git/config
> 3) Local level         : --local option. Specific to the current repository.  
       file> .git/gitconfig

Each level overrides values in the previous level: system -> global -> local  
<br>

```
$ git config --global user.name "your-name"
$ git config --global user.email your-email-address@~
$ git config --global init.defaultBranch main
$ git config --list
$ git config --list --show-origin
$ git config user.name
```
<hr>

## ✨Initializing a Repository in an Existing Directory
```
$ git init
```

## ✨Checking Repository Status
```
$ git status
```

## ✨Adding new file to be staged(tracked)
```
$ git add [file_name]   or   $ nano name-of-file.txt
```

## ✨Adding all files to be staged(tracked)
```
$ git add .
```

## ✨Unstaging a file
```
$ git rm --cached [file_name]
```

## ✨Ignoring a file
```
$ nano .gitignore

*.a          : ignore all files
!lib.a       : but do track lib.a even though ignoring .a files above
/TODO        : only ignore TODO file in the current dir, not subdir/TODO
build/       : ignore all files in any dir named build
doc/*.txt    : ignore doc/notes.txt, but not doc/server/arch.txt
doc/**/*.pdf : ignore all .pdf files in doc/ dir and anyu of its subdirs
```

## ✨Commit
```
$ git commit -m "commit message"
```

## ✨Change branch name
```
$ git branch
* master

$ git branch -m master main
$ git branch
* main

$ git status
On branch main
nothing to commit, working tree clean
```
