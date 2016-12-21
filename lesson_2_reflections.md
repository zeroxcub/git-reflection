## What happens when you initialize a repository? 
## Why do you need to do it?

- a `.git` folder is created to contain all metadata related to the repository
- allowing git to track file changes in that directory and save it as a commit
--------------

## How is the staging area different from the working directory and the repository?
## What value do you think it offers?

- staging area make it easy to bundle change of different file into one logical change and commit it
- staging area differ form working directory by that staging area contain all the change you want to commit but working directory may contain change that isn't part of a commit yet
--------------
## How can you use the staging area to make sure you have one commit per logical change?

adding only changes to be commited to the staging area and making it as small as possible

few things to note:
- after a commit and when the working directory (WD) is clean, the WD, staging area and the last commit should contain the same files
- you can see the difference between:
    - WD and staging area by `git diff`
    - staging area and last commit by `git diff --staged`
     

---------------
## What are some situations when branches would be helpful in keeping your history organized? How would branches help?

branch can help by making easier to work on different aspect of a project using the same repository
use it for :   
   - new feature
   - bug fix
   - experimental code

----------
## How do the diagrams help you visualize the branch structure?

by showing what commit is reachable by what (commit can only reach his parent)
use `git log --graph --oneline master branch1 branch2` to view a graph showing only reachable commit from master branch1 and branch2

----------
## What is the result of merging two branches together?

it merge the two commit of the branches automatically into a new commit at the tip of the checkedout branch by comparing the last commit of each branch to merge and its common parent using 
some rules to determine what files/lines to keep or delete:

- the files/lines in the parent and the two children is kept
- the files/lines added in one of the children is kept
- the files/lines deleted in one of the children is deleted
- for the other case git ask the code maintener with a merge conflict message

after a merge the log is rearranged using timestamp so use `git show` to view the difference between
a commit and its parent

----------
## What are the pros and cons of Git’s automatic merging vs. always doing merges manually?

- git allow you to take hand when merging is difficult without implying anything and give you the opportunity to discuss about the change to commit
- it add the **easy change** in the staging area and modify the conflicting file so that you cant change it at your convenience
and you have to commit the merge commit to merge the branch