Searching text in a file is a very common task. 

Vim allows you to search for a file by using `/` (forward slash) to search forward and `?` (question mark) to search backward in a file. Let's try it out.

Open the file again that you created:

```plain
vim new-file
```{{exec}}
```

**Basic Search**

Type `/` to enable search mode and type `li`

You will notice that the cursor points out the nearest matching string

Press `n` to jump to the next occurence or `N` to jump to the previous occurence

Next, type `?` to enable search mode again but backwards this time and type `li`

Press `n` or `N` to jump to the next occurence and notice that it will go backwards

You can use up/down arrow keys when you are in search mode to display your previous search strings

**Search Entire Word**

As you may notice, search command looks for a string pattern, not the entire word
to search the whole word, you need to enter `/\<line\>` to find `line` in the file

Vim allows us to search the current word that the cursor is pointing

Type `/` to enable search mode and type `li`

Now, press `*` (asterisk) to search the entire word which is `line` in our case
You can also press `#` (hash) to search backwards

**Ignore Case**

By default search is case-insensitive. It is possible to ignore case in a search by adding `\c` to the end of your search string

Type `/` to enable search mode and type `this`

It won't return any results

Type `/` again and type `this\c` this time and notice that search finds string `This` which has a capital letter

You can also ignore case indefinitely for the current session

Type `:set ignorecase` or `:set ic`

To revert it back, Type `:set noignorecase` or `:set noic`

To make it default for vim, you need to add it to `~/.vimrc` file

**Find and Replace**

last but not least, 


Vim lets you to move in a file by using keyboard shortcuts.
When you master these shortcuts, you won't want to use any other command line editor.
let's dive in!

First generate a file to work on with 100 lines:

```plain
for i in {1..100}; do echo "This is line $i" >> new-file; done
```{{exec}}
```

Open the file that you created:

```plain
vim new-file
```{{exec}}
```

Press `Esc`{{}} and type `:set number` to show the line numbers

As default we are in the first line. 
To get to the last line, enter `]]` or `G`

To get to the first line, enter `[[` or `gg`

Use keyboard shortcuts below to play around and get familiar:

| Shortcut Key | Function |
| :----------: | :------ |
| h	| moves the cursor one character to the left |
| j or Ctrl + J | moves the cursor down one line |
| k or Ctrl + P |	moves the cursor up one line |
| l |	moves the cursor one character to the right |
| 0 |	moves the cursor to the beginning of the line |
| $ |	moves the cursor to the end of the line |
| ^ | moves the cursor to the first non-empty character of the line |
| w |	move forward one word (next alphanumeric word) |
| W |	move forward one word (delimited by a white space) |
| 5w | move forward five words |
| b |	move backward one word (previous alphanumeric word) |
| B |	move backward one word (delimited by a white space) |
| 5b | move backward five words |

