# About *'Shell'*

## ✨What is Shell? 
> A ***shell*** is a type of computer program called a command-line interpreter  
> that lets Linux and Unix users control their operating systems with command-line interfaces.  
> Shells allow users to communicate efficiently and directly with their operating systems.  
> > Source: [What is Shell?](https://www.datacamp.com/blog/what-is-shell)

### <mark> *Shell* is *'an interface that allows users to communicate with operating systems'*. </mark>
<br>

## ✨How to use Shell?
> For Window, install and use [Git Bash](https://git-scm.com/).  
> For Linux/MacOS, search for "Terminal" in your apps and run.

<br>

## ✨Shell command
```
/                         (root)
.                         (current directory)
..                        (upper-level directory)
~                         (home of current user)
/[directory name]         (absolute path)
./[directory name]        (relative path)
../[directory name]       (relative path)
```
<br>

```
$ pwd
```
> ***'pwd'*** shows the current path in a hierarchical directory.
<br>

```
$ cd
```
> ***'cd'*** changes directory
<br>

```
$ ls
```
> ***'ls'*** lists files & directories
<br>

```
/bin                      (lists files in the /bin directory)
-l                        (lists files in the working directory in long format)
-l /etc /bin              (lists files in the /bin & /etc directory in long format)
-la ..                    (lists all files)
```
> These are used with 'ls'.
<br>

```
File Permissions      Owner   Group   Size(in bytes)   Modification Time   File Name

-rw-------         1  me      me      576              Apr 17 2019         weather.txt
drwxr-xr-x         6  me      me      1024             Oct  9 2019         web_page
-rw-rw-r--         1  me      me      276480           Feb 11 20:41        web_site.tar
```
> These are examples.
<br>

> If you want autocompletion, press 'tab' key.  
> If you want to do past commands, press '↑' key.  
> If you want to clear the shell, enter 'clear'.  
<br>

```
cp 
```
> ***'cp'*** copies files & directories
<br>

```
cp file1 file2            (copies contents of file1 into file2. If file2 doesn't exist, it is created. Otherwise, file2 is silently overwritten with the contents of file1)
cp -i file1 file2         (If file2 exists, the user is prompted before it is overwritten with the contents of file1)
cp file1 dir1             (copies contents of file1 inside of directory dir1)
cp -R dir1 dir2           (copies contents of directory dir1. If directory dir12 doesn't exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2)
```
> These are examples.


```
mv
```
> ***mv*** moves files and directories or rename them





