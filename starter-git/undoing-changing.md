#Undoing changing
- git restore file
# Bringing back the staged
- git restore --staged filename
- git reset HEAD filename(era feito antigamente)
# Correcting the last commit.
- git commit --amend -m "modify ..."
# Rocovering files
- git checkout (hash value) -- filename
# Removing unscanned files
- git clean -n will show you what will be removed
- git clean -f force removal of files.
# Reversing a commit
- git revert HEAD~value
- working tree must is cleanIT
- git log : HEAD-1, HEAD-2, etc...
