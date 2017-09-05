# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

I've been using linux a long time. I got this.

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls` 
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  


`ls  - list directory contents by name`  
`ls -a  - list hidden files as well`  
`ls -l  - long list showing attributes of entries`  
`ls -lh  - convert sizes to more compact form by unit`  
`ls -lah  - ditto for hidden files`  
`ls -t  - names sorted by date, newest first`  
`ls -Glp  - color-coded by file type and with a slash after subdirectories`  
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

I like -F for identifying files, -L for following links, -R for recursive subdirs and -r for sorting so the newest file is at the bottom. Sometimes -1 is useful if the list needs to be piped for more processing.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs allows you to run a command on multiple inputs, via standard input.  Here's a dumb example of doing a ls on just two files - colors and chsize:

`> echo colors chsize | xargs -n 1 ls -l`  
`-rwxr-xr-x  1 carlfrederick  staff  305 Mar 10  2014 colors`  
`-rwxr-xr-x  1 carlfrederick  staff  96 Mar  8  2014 chsize`  

 

