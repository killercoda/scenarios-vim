You will often need to find and replace a string in a file.

There is a command to do that in the whole form:
```
:[range]s/{pattern}/{string}/[flags] [count]
```

Vim lets you also use a different delimiter instead of `/` if you have it already in your search pattern. For example: `:s|foo|bar|` 

Please note that given parameters shown in brackets are optional.
Let's try it out.

&nbsp;

Open the file that you created:

```plain
vim new-file
```{{exec}}

In normal mode, type `:s/line/row/`

Notice that the first occurrrence of string `line` is replaced

To replace all occurrences in a line, you would use `:s/line/row/g` 

But the result won't change in our case, because we have the string `line` only once in each line

Add same string multiple times in a line and try it out if you wish

&nbsp;

When you want to find and replace all occurrences of a string in entire file, you need to use `%` (percentage character) in front of `s` to define the complete range

Type `%s/line/row/g` and notice that all occurrences of `line` have been replaced in the file

&nbsp;

**Ignore Case**

To ignore case in your search, use the `i` flag:

Type `:%s/this/that/gi` to replace all occurrences of `this` case insensitively with `that`

&nbsp;

**Search Range**

We can define a range of line by just giving it with a `,` (comma character) before `s`:

Type `:5,10s/line/LINE/g` to replace all occurrences of `line` with `LINE`

`.` (dot character) indicates the current line and `$` the last line

Type `:.,$s/this/those/i` to replace all occurrences of `this` with `those` from the current line to the end of the file. `i` is added to ignore case in the search

&nbsp;

You can test out a few different find and replace scenarios below

First type `:q!` to quit without saving and open the file again with its initial version:

```plain
vim new-file
```{{exec}}

&nbsp;

**Case:** Get to line 50 and replace all occurrences of `This` with `That` starting from the current line up to next 5 line

Type `:50` to get to line 50 and type `:.,+5s/this/That/i`

**Case:** Comment out the lines between 20-30 (in Vim you put a `#` in the beginning of a line to comment out as in python)

This is particularly important when you are dealing with configuration files in linux

Type `:20,30s/^/# /` as `^` denotes the beginning of a line

Type `:20,30s/^# //` to uncomment them










