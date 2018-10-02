# GIT

### Create a new branch and switch to it immediately

This shorthand will create and checkout in one.

```bash
$ git checkout -b <branch_name>
```

### Get the latest changes to the branch

Details here: http://longair.net/blog/2009/04/16/git-fetch-and-merge/

```bash
$ git fetch origin
$ git merge origin/develop
```

### Reset local branch changes / Set branch to exactly match the remote branch

```bash
$ git fetch origin
$ git reset --hard origin/develop
```

### Stage new and modified, without deleted

```bash
$ git add .
```

### Roll back the last commit but leave files intact

```bash
$ git reset --soft HEAD~1
```

### Push my feature branch back to origin
```bash
$ git push origin <branch_name>
```

### Merge two local branches - get a feature branch up-to-date

```bash
$ git checkout develop
$ git fetch origin
$ git merge origin/develop
$ git checkout <branch_name>
$ git merge develop
```

### Delete a remote branch

```bash
$ git push origin --delete <branch_name>
```

#### Rename the current local branch
```bash
$ git branch -m <new_branch_name>
```
