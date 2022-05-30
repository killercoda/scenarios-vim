You can also type `:wq` to save and quit which is equal to `:x`

If you just want to quit, just type `:q`

type `q!` if you want to quit without saving your changes.

&nbsp;

Open the file that you just created:

```plain
vim my-file
```{{exec}}

Type `o` to insert new line **below** the current line by also switching to insert-mode.

Now add some more text to the file, like `just landed`!

To get into command-mode press `Esc`{{}}

To save the file we need to type `:wq` and confirm with `Enter`{{}}

This will close Vim and save the file same as `:x`

&nbsp;

Open the file again:

```plain
vim my-file
```{{exec}}

press `Esc`{{}} and type `:q` without making any changes to quit.

Once again, open the file and make some changes. We want to quit this time with our changes to be ignored. 

You'll need to use it often when you accidentally changed in a file.

```plain
vim my-file
```{{exec}}

Type `O` (capital `o`) this time to insert new line **above** the current line and switching to insert-mode.

Now add some text and press `Esc`{{}} and type `:q`

Vim doesn't let you to quit because you didn't save your changes. 

type `:q!` to override and quit. Any changes you've made will be ignored.