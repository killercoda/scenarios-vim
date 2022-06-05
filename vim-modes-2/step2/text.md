Let's create a file with some content:

```plain
cat << EOF > new-file
Hello World,
This exercise is awesome!
I am learning a lot
I want to be a Vim master
And I'm feeling that I am very close to my goal!
Let's see if this text is long enough 
EOF
```{{exec}}

Open the file that you created:

```bash
vim new-file
```{{exec}}

>   You will notice that vim has a different appearance than before 

Press `v` to activate Visual mode in plain mode and you'll notice that text is highlighted as you move your cursor

This is how you make your text selection in a file in Visual mode

When you finished with your random selection, type `y` to copy(yank) the selection

Type `G` to get to end of file and click `p` to paste the selection

&nbsp;

**Comment out multiple lines**

>   You'll often need to comment/uncomment multiple lines in a config file. You can perform this operation conveniently in Visual mode 

Type `gg` to get to top and press `Shift + V` to activate Visual mode in block mode and notice that all text in the current line is selected

Type `2j` or use down-arrow key to select the first 3 lines

Type `:s/^/# ` to replace the first character with `# `

&nbsp;

**Sorting**

Make a reset first to undo all changes by typing `:u0`

Make sure you are on top or type `gg` to get to the beginning of file

Press `Shift + V` to activate Visual mode in block mode

Press `G` to select all text

Type `:sort ui` and notice that the text is sorted








