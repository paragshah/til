# Single Line Git Logs

View the last 20 commits of a branch in a single-line format:
```
git log --oneline --graph --decorate -n 20
```

Create an alias in your bash profile:
```
alias gl='clear;git log --oneline --graph --decorate -n 20;printf "\n"'
```

Then using terminal, enter `gl` to output the log. The output will look like:
```
* 6af36f1 (HEAD -> master, origin/master, origin/HEAD) Adding more bash commands
* eff1236 Add simple web server
* d66980e Add inspire by
* 08b7d7e Adding initial list of topics
* 3d4c8f1 Initial commit
```

