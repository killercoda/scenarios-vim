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

When you are done, Press `Esc`{{}} and type `:q!` to quit without saving.