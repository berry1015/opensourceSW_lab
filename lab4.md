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
/                         (root. 최상위 경로)
.                         (current directory)
..                        (upper-level directory)
~                         (home of current user. 홈 디텍토리.)
/[directory name]         (absolute path. 절대경로)
./[directory name]        (relative path. 상대경로)
../[directory name]       (relative path)
```
<hr>
<br>

```
$ pwd
```
> ***'pwd'*** shows the current path in a hierarchical directory
<hr>
<br>

```
$ cd
```
> ***'cd'*** changes directory
<hr>
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
> These are used with 'ls'
<hr>
<br>

```
File Permissions      Owner   Group   Size(in bytes)   Modification Time   File Name

-rw-------         1  me      me      576              Apr 17 2019         weather.txt
drwxr-xr-x         6  me      me      1024             Oct  9 2019         web_page
-rw-rw-r--         1  me      me      276480           Feb 11 20:41        web_site.tar
```
> These are examples
<hr>
<br>

> If you want autocompletion, press 'tab' key
> If you want to do past commands, press '↑' key
> If you want to clear the shell, enter 'clear'
<hr>
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
cp -R dir1 dir2           (copies contents of directory dir1. If directory dir2 doesn't exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2)
```
> These are examples
<hr>
<br>

```
mv
```
> ***'mv'*** moves files and directories or rename them
<br>

```
mv file1 file2            (If file2 doesn't exist, file1 is renamed file2. If file2 exists, its contents are replaced with contents of file1.)
mv -i file1 file2         (If file2 exists, the user is prompted before it is overwritten with the contents of file1)
mv file1 file2 dir1       (file1 & file2 are moved to directory dir1. If dir1 doesn't exist, mv will exit with an error)
mv dir1 dir2              (If dir2 doesn't exist, dir1 is renamed dir2. If dir2 exists, dir1 is moved within directory dir2)
```
> These are examples
<hr>
<br>

```
rm
```
> ***'rm'*** deletes files and directories <mark>permantely and irreversevely</mark>
<br>

```
rm file1 file2            (delete file1 & file2)
rm -i file1 file2         (user is prompted before each file is deleted)
rm -r dir1 dir2           (dir1 & dir2 are deleted along with their contents)
```
> These are examples
<hr>
<br>

```
mkdir
```
> ***'mkidr'*** makes a new directory
<hr>
<br>

```
*                         (all filenames)
g*                        (all filenames that begin with the character 'g')
b*.txt                    (all filenames that begin with the character 'b' and end with the characters '.txt')
Data???                   (any filename that begins with the characters "Data" followed by exactly 3 more characters)
```
> These are ***'wildcard'*** 
<hr>
<br>

```
cp *.txt text_files       (copy all files in current working dir with names ending with characters ".txt" to an existing dir named text_files)
mv dir1 ../*.bak dir2     (move subdirectory dir1 and all the files ending in '.bak' in current working dir's parent dir to an existing dir named dir2)
rm *~                     (delete all files in current working dir that end with the character '~'. Some applications create backup files using this naming scheme. Using this command will clean them out of a dir.)
```
> These are examples of ***'cp, mv, rm'***
<hr>
<br>

```
help
```
> ***'help'*** shows the documents included in the Git.  
> You can get help when there is something you don't know while using git
<hr>
<br>

```
man
```
> ***"man'*** is used to access the manual pages for other commands
<hr>
<br>

```
exit
```
> ***"exit'*** is used to leave the manual page viewer (like less or more) and return to the command line.
<hr>
<br>
