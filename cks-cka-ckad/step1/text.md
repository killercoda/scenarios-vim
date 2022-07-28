
> The following settings **will already be configured** in your real exam environment in ~/.vimrc. But it can never hurt to be able to type these down

We look at important Vim settings if you like to work with YAML during the K8s exams.


### Settings
First create or open (if already exists) file `.vimrc`:

```plain
vim ~/.vimrc
```{{exec}}

Now enter (in insert-mode activated with `i`{{}}) the following lines:

```plain
set expandtab
set tabstop=2
set shiftwidth=2
```

Save and close the file by pressing `Esc`{{}} followed by `:x`{{}} and `Enter`{{}}.


### Explanation
Whenever you open Vim now as the current user, these settings will be used.

If you ssh onto a different server, these settings will **not** be transferred.

Settings explained:

```plain
expandtab: use spaces for tab
tabstop: amount of spaces used for tab
shiftwidth: amount of spaces used during indentation
```
