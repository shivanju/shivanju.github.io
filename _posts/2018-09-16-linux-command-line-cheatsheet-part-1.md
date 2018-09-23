---
layout: post
title: Part-1 How to become a command line ninja?
tags: [Linux, Command line, cli, Unix, Shell, Bash]
---

Becoming a ninja is pretty easy task; especially if it's the command line ninja. Just equip the right tools, know how to read the manual for those tools and some practice. All you have to do is stick to the plan.  
Remember this is not a comprehensive guide for the command line but knowing this will serve your purpose 87% of the time.  
In part one we will learn about some very frequently used commands and utilities. Part two will be about more sophisticated commands related to system, network, processes etc. Now let's see what tools we've got...

### __Legends__:
__C__ : Ctrl/Command key
__M__ : Mod key/Alt

### 1. __Moving around__
__`C-a`__ : _beginning-of-line_  
Moves the cursor to the start of current line.

__`C-e`__ : _end-of-line_  
Moves the cursor to the end of current line.

__`C-l`__ : _clear-screen_  
Clears the screen.

__`M-f`__ : _forward-word_  
Moves the cursor to the end of current or next word.

__`M-b`__ : _backward-word_  
Moves the cursor to the start of current or previous word.

### 2. __History__
__`C-r`__ : _reverse-search-history_  
Search backward starting at the current line and moving ‘up’ through the history as necessary

__`unbound`__ : _history-search-forward_  
Search forward through history for the commands which exactly match the characters between start of the line and the cursor position

__`unbound`__ : _history-search-backward_  
Search backward through history for the commands which exactly match the characters between start of the line and the cursor position

Till here all the previous commands are the part of [GNU readline][gnu-readline] and they can be remapped. Go check the whole list, may be you'll find something interesting.


Here is one example for remapping the _history-search-forward_ and _history-search-backward_ command. And I can say for sure that this 
one's gonna stick with you for a long time. We will map UP and DOWN arrow keys to these commands respectively. By default these keys search forward/backward for one command at a time.

Create a file with the name __.inputrc__ in your home directory or wherever you usually put your other _rc_ (.bashrc, .vimrc etc.) files
and paste these lines. Restart your shell and you're ready to go.

```
"\e[A": history-search-backward
"\e[B": history-search-forward
```

### 3. __Utilities__
In this section we'll see some ubiquitous command line utilities. You'll recognize most of them but you may find some new ways to use them. Again this will not be a comprehensive manual for all utilities, but will be more than enough to get you started.
I would suggest that you try and experiment with these commands as you read to get some more familiarity.

a. __man__: Opens up the manual page of a command.  
```
$ man man
```
b. __apropos__: Searches the manual pages containg the keywords.
```
$ apropos apropos
apropos (1)          - search the manual page names and descriptions
```
c. __whatis__:  Displays one-line manual page descriptions.
```
$ whatis whatis
whatis (1)           - display one-line manual page descriptions
```
d. __Directories & files__:
  * __ls__: List the contents of a directory. Common flags are __-l__ (long list), __-a__ (all), __-h__ (human readable), __-t__ (sort by modification time)
  ```
  $ ls
  file1
  file2
  directory1
  ```
  * __cd__: Change directory. Common shell expansions are __~__ ($HOME), __-__ (last location), __.__ (current directory), __..__ (previous directory)
  ```
  $ cd ~/Documents
  ```
  * __pwd__: Print working directory
  ```
  $ pwd
  /home/Alice/Documents/foo/bar
  ```
  * __mkdir__:  Make directories. Common flag is __-p__ (make parent directories as needed)
  ```
  $ mkdir Games/rpg
  ```
  * __rmdir__: Remove empty directories. Common flag is __-p__ (remove directory and its parents)
  ```
  $ rmdir -p Games/rpg
  ```
  * __touch__: Create file or change file timestamps
  ```
  $ touch file
  ```
  * __rm__: Remove files or directories. Common flags are __-r__ (recursive), __-f__ (force), __-i__ (prompt before every removal)
  ```
  $ rm -rf /home/Alice/Documents/foo/bar
  ```
  * __cp__: Copy files and directories from SOURCE to DESTINATION. Common flag is __-r__ (recursive)
  ```
  $ cp /home/Alice/Documents/file1 /path/to/destination
  ```
  * __mv__: Move/Rename files. Common flag is __-r__ (recursive)
  ```
  $ mv /home/Alice/Documents/file1 /path/to/destination
  ```


e. __File contents__:
  * __cat__: Concatenate files and print the content on the standard output
  ```
  $ cat file1 file2
  ```
  * __head__: Output the first few lines of files. Common flag is __-n__ (number of lines), default is __10__
  ```
  $ head -n3 file
  ```
  * __tail__: Output the last few lines of files. Common flags are __-n__ (number of lines), __-f__ (follow the output if file grows)
  ```
  $ tail -f foo.log
  ```
  * __less__: View the contents of a text file one screenful at a time
  ```
  $ less file
  ```
That's all folks for this part. I'll keep updating this part if I find something that should belong here.


[gnu-readline]: https://www.gnu.org/software/bash/manual/html_node/Bindable-Readline-Commands.html
