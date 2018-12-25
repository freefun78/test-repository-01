# Test Git (Python tutorial RESTAPIFLASK-Udemy)

## Create key :
ssh-keygen

This will create private and public key in ~/.ssh
The directory is referenced for key access by default.

## Add Key in GIT :
Open public key and copy paste the content to profile > SSH & GPG Keys 
section.

## To start git
Goto directory and issue git init.

## To check git status
git status

## To add git tracking
git add [file ... | -A]

## commit
git commit

## to merge to github
git remote add origin [get url from https | ssh from github repository 
clone or download drop button]

## to remove source
git remote remove origin

## remote status
git remote -v

## push
git push --set-upstream origin [...]
git push

## create branch
git branch [branch_name]

## switch branch (checkout)
git checkout [branch_name] 

## Active branch
git branch

## Synch with upstream/remote check if there' any changes
git pull


## Merge with master (switch to branch first)
git checkout [branch_name}
git merge master

## Push to upstream
git push --set-upstream origin [branch_name]

## Workflow
in general the workflow is as follow :
1. Create branch -> git branch [branch name]
2. Switch branch -> git checkout [branch name]
3. Make changes
4. Add tracking on those changes -> git add -A
5. Try to merge if -> git merge master (goto parent branch and do a get 
pull if necessary prior to check if the parent branch has not changed)
6. Resolve any conflic and goto step 4.
7. If no conflict, commit -> git commit
8. Push the changes to github -> git push --set-upstream origin [branch 
name]. At this point new branches will be created @github.
9. Goto github and create pull request for review by other team members.
10. make necessary changes if there's any comment and goto step 4.
11. The designated team members can merge the pull request (in github 
page).
12. Delete branch if desired.

