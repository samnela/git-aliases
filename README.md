# Git Aliases

Some very useful aliases

How to set a alias ?

git config --global alias.$name  $command

<h2>Aliases </h2>

<h3>git Stash </h3>
git config --global alias.stsh 'stash --keep-index'

git config --global alias.staash 'stash --include-untracked'

git config --global alias.staaash 'stash --all'

<h3> git Branch </h3>

git config --global alias.br  branch

git config --global alias.del 'branch -D'

git config --global alias.dela '!f(){ git branch -D $2 && git push $1 -d $2 ; }; f'

<h3> git Log </h3>

git config --global alias.last 'log -1 HEAD'

<h3> git Wip </h3>

git config --global alias.wip "for-each-ref --sort='authordate:iso8601' --format=' %(color:green)%(authordate:relative)%09%(color:white)%(refname:short)' refs/heads"
