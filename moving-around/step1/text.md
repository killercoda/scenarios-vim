Vim lets you to navigate in a file by using keyboard shortcuts.

When you master these shortcuts, you won't want to use any other command line editor.

Let's dive in!

&nbsp;

First generate a file to work on with 100 lines:

```plain
for i in {1..100}; do echo "This is line $i" >> new-file; done
```{{exec}}

Open the file that you created:

```plain
vim new-file
```{{exec}}

Vim has multiple modes, but we will focus first to **normal mode**

This mode is the default mode and it can always be activated by pressing `Esc`{{}}

In Vim, almost all operation commands are performed in normal mode

**Important Note:** you can undo whenever you need it in normal mode by pressing `u` 

&nbsp;

Press `Esc`{{}} and type `:set number` to show the line numbers

You can move to a line by just entering the line number in normal mode

Type `:30` to jump to line 30

It is also possible to jump directly to a character in a file

Type `:goto 700` to jump to 700. character
