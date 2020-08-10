# vim Cheat Sheet :shit:

Tend to forget simple commands that I don't use so much and for improved productivity decided to write them down.

## Moving around

`gg` beginning of file

`GG` beginning of end of file

`$` end of line

`^` beginning of line

`g_` last non-whitespace character

`g$` end of screen 

## Show hidden characters

`:set list` shows

`:set nolist` hides hidden characters

## Show line numbers

`set number`

`set nonumber`

## Delete (a) word(s)

`dw` deletes word starting from cursor

`daw` deletes a whole word

`df ` deletes from cursor until next space _or_ any other char instead of space, e.g.:

`df.` deletes whole sentence, until the dot.

### Change a word

`caw` changes a word (deletes and puts into insert mode)

### Change in range

`:5,12s/foo/bar/g` 	Change each 'foo' to 'bar' for all lines from line 5 to line 12 (inclusive).

## Delete every other line

E.g. when copying from a table and editor parses second row onto a new line.

Works like this: `:[range]g/pattern/cmd`

To delete all even lines:

`:g/^/+d`

To delete all odd lines [this guy](https://til.hashrocket.com/posts/c81edb64c0-delete-every-other-line) states:

`:gg/^/+dd` (?) 

[Delete line this many times](https://stackoverflow.com/questions/1946738/vim-how-to-delete-every-second-row)

`gg` `qq` cursor down & `dd` `q` `10@q`

## TODO:

* Figure out how to delete all odd lines.
