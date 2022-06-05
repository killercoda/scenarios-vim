Manipulating text in Vim with some handy commands in Normal mode can save you a tons of time. 

Let's create a longer text file with more content:

```plain
cat << EOF > long-file
Hello World,
This exercise is still awesome!
I am learning a lot
I want to be a Vim master
And I'm feeling that I am very close to my goal!
Let's see if this text is long enough 
EOF
```{{exec}}

Open the file that you just created:

```bash
vim long-file
```{{exec}}

First type `:set number` to show the line numbers

Type `O` to enter a new line on top by switching to insert mode and write some text 

&nbsp;

**Delete**

Press `Esc`{{}} and type `dd` to delete the line

Press `u` to undo your changes and make sure that you are still on line 1 (You can always type `gg` to get to the top)

Type `3d` and press `Enter` to delete the first 4 lines. Notice that deleting is a 0 indexed operation with `d` command so try with `1d` and notice that it will remove 2 lines below

Type `D` to remove the content of the line but not the line itself

**Delete all lines in Vim**

Type `gg` to get to first line

Type `dG` to clear the file completely

&nbsp;

You can just try out more sophisticated delete operations:

| Command | Description |
| :----------: | :------ |
| `d<left-arrow>` | Delete current and left character |
| `d<right-arrow>` | Delete current and right character |
| `d<up-arrow>` | Delete current and upper line  |
| `d<down-arrow>` | Delete current and bottom line |
| `d$` | Delete from current position to end of line |
| `d^` | Delete from current backward to first character |
| `dO` | Delete from current backward to beginning of line |
| `dw` | Delete current to end of current word |
| `db` | Delete current to beginning of current word |

&nbsp;

Try it out and when you are ready:

Press `Esc`{{}} and type `:q!` to quit without saving




