We've covered most functionalities of Normal mode in previous scenarios

Let's focus on Insert mode and create a new file with some content to work on:

```plain
cat << EOF > new-file
Hello World,
This exercise is awesome!
EOF
```{{exec}}

Open the file that you created:

```bash
vim new-file
```{{exec}}

>   You will notice that vim has a different appearance than before

Click `i` to activate Insert mode. You can add/delete text as you want

Press `Esc`{{}} and press `u` to undo your last change

&nbsp;

There are also another ways to activate Insert mode:

| Command | Description |
| :----------: | :------ |
| `o` | Insert new line **below** the current line and switch to insert-mode |
| `O` | Insert new line **above** the current line and switch to insert-mode |
| `a` | Append **after cursor** and switch to insert-mode |
| `A` | Append **at end of line** and switch to insert-mode |
| `s` | Delete the character cursor is **currently on** and switch to insert-mode |
| `C` | Delete all **after cursor position** and switch to insert-mode |

&nbsp;

Try it out and when you are ready:

Press `Esc`{{}} and type `:q!` to quit without saving







