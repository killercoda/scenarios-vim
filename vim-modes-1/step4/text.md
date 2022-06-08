Let's continue with copy, cut & paste commands in Vim

Open long-file that you created:

```bash
vim long-file
```{{exec}}

First type `:set number` to show the line numbers

Type `G` to get to the end of the file and type `o` to enter a new line by switching to Insert mode and write some text

**Copy, Cut & Paste**

Press `Esc`{{}} and type `yy` to copy the line (y is short for yank)

Type `:2` to jump to line 2 and type `p` to paste the content to line 3

>   Repeat the operation by pressing `dd` to cut a line and `p` to paste the content

&nbsp;

Type `:u0` to **undo all changes** since opening to reset

Type `:4` and get to line 4 and type `3yy` to copy the current and next 2 lines

Type `gg` to get to the top and type `P` to paste these 3 lines before the cursor

Replace `3yy` with `3dd` to cut instead of copy and reply the operation if you wish

&nbsp;

Again, refer to the table below for more sophisticated copy operations in Vim

| Command | Description |
| :----------: | :------ |
| `y$` | Copy all from current to end of line |
| `y^` | Copy all from current to start of line |
| `yw` | Copy to the start of next word |
| `yiw` | Copy the current word |