## When would you want to use a remote repository rather than keeping all your work local?

- when you want to share your code with someone else or to a team
- when you want a **anywhere** and **anytime** accessible safe repository
    
### git remote command

- `git remote` list all remote repository (like `git branch` to list all branches)
- `git remote add origin #git_remote_url` add a remote repository called origin (whatever name you wish) at the url

-----------------

## Why might you want to always pull changes manually rather than having Git automatically stay up-to-date with your remote repository?
to avoid merge conflict in an intermediate repository state

### git push/pull command

push or pull to/from the remote repository using
`git push/pull origin master` where the origin is the name of the remote repository and the branch you want to push/pull

-----------------

## Describe the differences between forks, clones, and branches.  
When would you use one instead of another?

- a branch is only on the local repository, it mean to make another path in th git history for experimental change, another feature and so on
(it can be pushed on the remote repository though)
- a clone is a local copy of any repository (remote or local) it has the same history log as the original and you can pull update from the remote to yours 
- a forks is like a clone, it's a GitHub related concept. It's basically:
    - clone a repository inside GitHub
    - link the clone to the original repository
    - then you can clone the fork into your local repository
you can't push nor pull update to the original forks, you only have a link to it and only push pull to you forks on GitHub

So clone if you intend to receive update an push update, fork if you want a standalone repository for your self

-----------------

## What is the benefit of having a copy of the last known state of the remote
stored locally?

    Fill in your answer here
    
-----------------

## How would you collaborate without using Git or GitHub?  What would be easier,
and what would be harder?

    Fill in your answer here

------------------

## When would you want to make changes in a separate branch rather than directly in
master?  What benefits does each approach have?

    Fill in your answer here
