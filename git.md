# Git Cheat Sheet :shit:

Tend to forget simple commands that I don't use so much and for improved productivity decided to write them down.

## Resolving Conflict

To make life easier for oneself, have different branches on different computers -- makes resolving easier, maybe.

### Merge Conflict

```bash
On branch master
Your branch and 'origin/master' have diverged,
and have 1 and 1 different commits each, respectively.
```

See where you diverged:

`git reflog`

More visual one-liner:

`git log --graph --decorate --oneline $(git rev-list -g --all)`

#### To Revert

`git revert SHA` from `git log --graph --decorate --oneline`

#### To Reset

##### Soft

This will keep the reference logs:

`git reset --soft HEAD@{n}`

`n` is from `reflog`

##### Hard

Hard reset will discard the reference logs.

`git reset --hard HEAD@{n}`

## Rename repository

0. Rename on Remote host, e.g. https://github.com/akerge/cheat-sheets

0. Rename directory on local host

0. Set new URL using git

`git remote set-url origin git@github.com:akerge/cheat-sheets.git`

#### Choose Your Own Adventure

To have an adventure, follow [this](http://sethrobertson.github.io/GitFixUm/fixup.html)
