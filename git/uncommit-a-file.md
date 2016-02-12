# Uncommit a file

Sometimes, you may need to uncommit a single file from your local repo. You can do this using `git checkout`:
```
git checkout HEAD^ -- <path/filename.ext>
```

Create an alias in your bash profile:
```
alias guc=git_uncommit_file

# contents of git_uncommit_file function:
git_uncommit_file() {
  if [ $# -eq 0 ]
    then
      echo "No arguments supplied."
  else
    git checkout HEAD^ -- $1
    printf "\n"
    echo "$1 now uncommitted."
    printf "\n"
  fi
}
```

Then enter `guc <path/filename.ext>` to uncommit the file.
