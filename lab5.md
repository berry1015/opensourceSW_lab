# About *'Shell'* (2)

## ✨Standard Output
> Standard output is <mark>***screen***</mark>.  
> Can redirect output using <mark>***'>'***</mark> after a command to create & save the output in a file.  
> Command <mark>***'cat'***</mark> displays content of a text file.  
> Using <mark>***'>>'***</mark> appends output to an existing file if it already exists, or create & write to a new file.
<br>

## ✨Standard Input
> Standard input is from <mark>***keyboard***</mark>.  
> Can redirect input from a file using <mark>***'<'***</mark>.  
> Can mix '<' and '>' together in a single line.  
<br>

## ✨Pipelines "|"
> A sequence of one or more commands separated by '|'.   
> Ex) com1 | com2 | com3 | ...  
> Press 'q' key to exit screen.
<br>

## ✨Expansion
> <mark>***'echo'***</mark> repeats that you write, name of files, or present directory.
```
$ echo print out the text
print out the text

$ echo *
README.md file_list.txt test.sh words.txt

$ echo ~
/Users/(name)
```
<br>

## ✨Backslash '\\'
> Can be used to ignore line change in command to enter a long command in multiple lines.
<br>

## ✨Permissions
> Files and directories ahve a permission assigned differently to owner/group/others.
```
$ -rwxrwxrwx

File type> -: Indicates regular file / d: Indicates directory
1st rwx: Read, write, execute permissions for the file owner
2nd rwx: Read, write, execute permissions for the group owner of the file
3rd rwx: Read, write, execute permissions for all other users
```
<hr>

> <mark>***'chmod'***</mark> changes permissions.
```
$ chmod 600 README.md

6= 110= rw- for owner
0= 000= --- for group
0= 000= --- for others
```
<br>

> **Values & Meanings**
```
777 (rwxrwxrwx)
No restrictions on permissions. May do anything. Generally not d desirable setting.  

755 (rwxr-xr-x)
File's owner may read, write, and execute. Others may read and execute. Common settings.

700 (rwx------)
File's owner may read, write, and exevute. Nobody else has any rights. Useful for keeping private.

666 (rw-rw-rw-)
All users may read and write the file.

644 (rw-r--r--)
Owner may read and write, while others may only read. Common setting for only the owner may change.

600 (rw-------)
Owner may read and write. Others have no rights. Common setting for owner wants to keep private.
```
<br>

## ✨Superuser
> Superuser has all system administration authority.  
> Some commands need superuser's privilleges.  
> Use <mark>***'sudo'***</mark> if you are superuser.  
> Type 'exit' to get out of a session.
<br>

## ✨Text Editors
![image](https://github.com/user-attachments/assets/cf8a2b58-2f18-4b17-ad0f-eb12f7a40e67)
🔗[Here is the Source link!](https://linuxcommand.org/lc3_wss0010.php)

<br>

> If you want to write and run a shell script with nano, write below:
```
$ nano myscript.sh 
```
<br>

> Type <mark>***'history'***</mark> to see previous command history or save it to a text file.
<br>

## ✨wget
> Download files from the internet directly to your active dir.
<br>

## ✨curl
> Fetching, uploading, and managing data over the internet
```
$ curl [options] [URL]
```
<br>

## ✨grep (Global Regular Expression Print)
> Searching text within files.  
> ex) grep "search_term" file.txt  
> => Searches for the exact 'search_term' within 'file.txt' and prints matching lines.
<br>

**Command options**
> '-i': Case-insensitive search (finds "apple" and "Apple")  
> '-v': Invert the match (finds lines ***not*** containing the search term)  
> '-n': Display line numbers along with matching lines  
> '-r': Recursive search (searches through all files in a dir and its subdir)
<br>

Supports powerful regular expressions for more complex searches.
> '.*'    : Matches any character('.') zero or more times('\*')
> '\d'    : Matches any digit(0-9)
> '[abc]' : Matches any single character within the brackets
> '^'     : Matches the beginning of a line
> '$'     : Matches the end of a line
  
