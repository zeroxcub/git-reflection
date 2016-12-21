## manual commit

### pros:
 - fine tuned commit organised logicaly
 - no half baked commit if made correctly

### cons:
 - may forget to commit
 - commit may be too broad and lost logical meaning
----------------
## multi-file commit
make easier to group, track and commit related to logical change to different files

## using git to view history
- use `git log --stat` to have a global view of commit history and changes

- use `git diff #id_commit1 #id_commit2` to view all  change on all file (ie: logical change) between two commit 
----------------
## using git to view history
- use `git log --stat` to have a global view of commit history and changes

- use `git diff #id_commit1 #id_commit2` to view all  change on all file (ie: logical change) between two commit 
- after a `git merge` the log is arranged in ascending fashion based on commit time stamp and therefore
commit doesn't always show as *parent<--children* so to view the difference between a commit and its parent 
we use `git show #commit_id`
---------------
## efficiency by having entire history available

- trace change over time
- revert to a particular version easily
----------------
## How might using version control make you more confident to make changes that could break something?

- I know that the last (working) code are always there if I made a mistake
----------------
## diff
### make viewing change between file a breeze
- a minus (-) mean the old file a plus (+) the new file
- show change in a chunk (hunk) to provide context like so

    `@@ -6,4 +6,4 @@`

    `-6` mean from old file, `+6` mean from new file both at line 6 provided with 4 line of context to help search semantic bug
- make typo easier to spot
- make easier to understand last edit semantic
----------------
