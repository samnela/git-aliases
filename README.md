# Git Aliases

Some very useful aliases

How to set a alias ?
```bash
git config --global alias.$name  $command
```

### git Stash 
```bash
git config --global alias.stsh 'stash --keep-index'

git config --global alias.staash 'stash --include-untracked'

git config --global alias.staaash 'stash --all'
```

### git Branch
```bash
git config --global alias.br  branch

git config --global alias.del 'branch -D'

git config --global alias.dela '!f(){ git branch -D $2 && git push $1 -d $2 ; }; f'
```

### git Log
```bash
git config --global alias.last 'log -1 HEAD'
```
### git Checkout
```bash
git config --global alias.new 'checkout -b'
```

### git Wip
```bash
git config --global alias.wip "for-each-ref --sort='authordate:iso8601' --format=' %(color:green)%(authordate:relative)%09%(color:white)%(refname:short)' refs/heads"
```