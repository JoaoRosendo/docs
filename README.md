# Personal documents

## Linux Aliases

```
alias retest='gh pr comment $(git rev-parse --abbrev-ref HEAD) --body "retest"'
alias branch='git branch'
alias switch='git switch'
alias amend='git add . && git commit --amend --no-edit && git push -f && sleep 3 && retest'
alias diff='git diff'
alias rebase='git pull && git checkout master && git pull && git switch - && git rebase master && git push --force'
alias master='git switch master && git pull'
alias status='git status'
alias flake8='flake8 --max-line-length=119'
alias push-gerrit='git push origin HEAD:refs/for/master && echo -e "\nCommit ID:" && git rev-parse HEAD'
alias merge='git add . && git commit --amend --no-edit && git push -f'
```
