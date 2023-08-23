# Git

## Squashing commits

To squash the last 3 commits into one:

```git reset --soft HEAD~3```

Write the new commit message

```git commit -m "New message for the combined commit"```


### Pushing the squashed commit

#### If the commits have been pushed to the remote:

```git push origin +name-of-branch```
The plus sign forces the remote branch to accept your rewritten history, otherwise you will end up with divergent branches

#### If the branch has not been pushed to the remote:

```git push origin name-of-branch```
