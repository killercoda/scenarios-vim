Vim has multiples modes to operate. We will focus on the most used ones as listed below:

| Mode | Description |
| :----------: | :------ |
| Normal	| Default mode for navigation and manipulation of text and it can always be activated by pressing `Esc`{{}} |
| Insert	|  Used for inserting/manipulating the text by using all keyboard keys. Not any Normal mode commands is active in this mode |
| Visual	| Used for navigation and manipulation of text selections. Allows the use of most Normal mode commands on selected text |

>   It is important to note that, in Vim, almost all operation commands are performed in **Normal mode**

In this scenario, we are going to install some vim plugins to change the visual appearance of vim, to be able to better understand how modes are functioning:

```bash
git clone --depth=1 https://github.com/amix/vimrc.git ~/.vim_runtime
```{{exec}}

```bash
sh ~/.vim_runtime/install_awesome_vimrc.sh
```{{exec}}


