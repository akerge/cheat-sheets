# bash  Cheat Sheet :shit:

Tend to forget simple commands that I don't use so much and for improved productivity decided to write them down.

## find

Basic syntax:

`find [from] [what]`

Symbolic links in currend directory:

`find . -maxdepth 1 -type l -ls`

### Folders

`find [from] -name "folder-name"`

`find [from] -type d "folder-name"`

## diff & patch

`-u` stands for unified context (easier to read)

`diff -u original_file file_to_compare > output.patch`

`-b` backs up the file to be patched

`patch -b file_to_be_patched patch.file`

## links

Symbolic link

`ln -s /where/to /link/location`

## list

List as a column:

`ls -1`

## get public keys

`wget https://github.com/akerge.keys`

## change ip

`ip addr #.#.#.#/# dev eth#`

`ip link set eth# down/up`

in Ubuntu it's `/etc/netplan.yaml`, fiddle with it and then `netplan apply`


