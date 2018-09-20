---
layout: post
title: How to become a command line ninja?
tags: [Linux, Command line, cli, Unix, Shell, Bash]
---

Becoming a ninja is pretty easy task; especially if it's the command line ninja. Just equip the right tools, know how to read the manual for those tools and some practice. All you have to do is stick to the plan.  
Remember this is not a comprehensive guide for the command line but knowing this will serve your purpose 87% of the time.  
Now let's see what tools we've got...

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
Here is the one example for remapping the _history-search-forward_ and _history-search-backward_ command. And I can say for sure that this 
one is gonna stick with you for a long time. We will map UP and DOWN arrow keys to these commands respectively. By default these keys search forward/backword for one command at a time.

Create a file with the name __.inputrc__ in your home directory or wherever you usually put your other _rc_ (.bashrc, .vimrc etc.) files
and paste these lines. Restart your shell and you're ready to go.

```
"\e[A": history-search-backward
"\e[B": history-search-forward
```

### 3. __Utilities__
Now let's see some ubiquitous command line utilities. You'll recognize most of them but you may find some new ways to use them.


[gnu-readline]: https://www.gnu.org/software/bash/manual/html_node/Bindable-Readline-Commands.html