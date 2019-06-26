# Git Cheat Sheet :shit:

Tend to forget simple commands that I don't use so much and for improved productivity decided to write them down.

## Resolving Conflict

First of all, have different branches on different computers -- makes resolving easier.

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

#### To Reset

##### Soft

This will keep the reference logs:

`git reset --soft HEAD@{n}`

`n` is from `reflog`

##### Hard

Hard reset will discard the reference logs.

`git reset --hard HEAD@{n}`
