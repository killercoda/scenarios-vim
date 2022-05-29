Searching text in a file is a very common task. 

Vim allows you to search for a file by using `/` (forward slash) to search forward and `?` (question mark) to search backward in a file. Let's try it out.

&nbsp;

Open the file again that you created:

```plain
vim new-file
```{{exec}}
```

**Basic Search**

Type `/` to enable search mode and type `li`

You will notice that the cursor points out the nearest matching string

Press `n` to jump to the next occurrence or `N` to jump to the previous occurrence

Next, type `?` to enable search mode again but backwards this time and type `li`

Press `n` or `N` to jump to the next occurrence and notice that it will go backwards

You can use up/down arrow keys when you are in search mode to display your previous search strings

&nbsp;

**Search Entire Word**

As you may notice, search command looks for a string pattern, not the entire word
to search the whole word, you need to enter `/\<line\>` to find `line` in the file

Vim allows us to search the current word that the cursor is pointing

Type `/` to enable search mode and type `li`

Now, press `*` (asterisk) to search the entire word which is `line` in our case
You can also press `#` (hash) to search backwards

&nbsp;

**Ignore Case**

By default search is case-insensitive. It is possible to ignore case in a search by adding `\c` to the end of your search string

Type `/` to enable search mode and type `this`

It won't return any results

Type `/` again and type `this\c` this time and notice that search finds string `This` which has a capital letter

You can also ignore case indefinitely for the current session

Type `:set ignorecase` or `:set ic`

To revert it back, Type `:set noignorecase` or `:set noic`

To make it default for vim, you need to add it to `~/.vimrc` file

&nbsp;

Press `Esc`{{}} and type `:q!` to quit without saving