# vim Cheat Sheet :shit:

Tend to forget simple commands that I don't use so much and for improved productivity decided to write them down.

## Delete every other line

E.g. when copying from a table and editor parses second row onto a new line.

Works like this: `:[range]g/pattern/cmd`

To delete all even lines:

`:g/^/+d`

To delete all odd lines [this guy](https://til.hashrocket.com/posts/c81edb64c0-delete-every-other-line) states:

`:gg/^/+dd` (?) 

## TODO:

* Figure out how to delete all odd lines.