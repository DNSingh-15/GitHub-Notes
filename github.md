## Git  commands 

### normal commands
```
1. git pull origin mein =>  merging code from main branch
   Git pull =>  merging code from current branch only
2. git commit -m “Initial commit” => first commit
3. git push
4. git switch => undo any changes you make and return to your previous branch
   git switch {branch name} => undo any changes you make and return to selected branch
5. git checkout => changing the branches.
for moving the branches we can use -- `git switch` and `git chekcout` both
```
  
### 1 (a). git fetch
     Git fetch only downloads latest changes in to local repository.
     Git fetch allows us to review and merge manually at a letter time using git merge.
     It doesn’t change anything in our directory

### 1 (b). git pull
     It downloads latest changes into our local repository
     It also automatically merges changes into our working directory.
     It doesn’t give a chance to review before merging

   ```
      git pull = git fetch + git merge
   ```
### 1 (c) git reset --hard ORIG_HEAD
     it is used for remove the current pull request that is not commited 

### 2. git log 
```
git log => git log command will give commit history

Git log —oneline => git log —oneline command will give commit history in one line
```

### 3. git revert Commit-id
```
     We can undo a particular commit by using git revert commit-id
     After  revert commit-id command we have to do => press scape and : ( colan ) wq ( it will looks like :wq => that is write and quit )
     And it will not remove that commit from the commit history. But it will give a new commit 
```
### 4. git stash
```
  a. git stash
     It is a temporary storage
     What ever changes we have made in our working directory that we can store into a storage by using git stash.
     Hum stash usi file ko kr sket hai jise humne abhi tak commit ni kiya hai 
  b. Git Stash List => We can check stash area by using git stash list
  c. Git Stash Apply =>  1.This command will give our latest code from that temporary storage 
                       2. That code is also present in the stash area
  d. Git Stash Clear => we can clear stash area ( temporary storage ) by using git stash clear
  e. Git Stash drop ( git stash drop 0 or etc ) => We can clear a particular file by using `git stash drop fileNumber( 0 or 1 or etc )`
  f. Git Stash Pop => git stash pop command helps us to remove latest file from the stash area
```

### 5 (a). cherry pick.
   Cherry picking is the act of picking a commit from a branch and applying it to another branch
   ```
  a.  git checkout brach-name ( where we want the commit )
  b. git fetch origin dev ( branch name from where we want the code into our local branch )
  b.  git cherry-pick  commit-id	
   ```
### 5 (b). Merge Abort
   ```
     git merge —abort  => this command remove the latest changes 
   ```

### 6 . synch issue => incomming and outgoing chnages in the same time 

```
git fetch origin

git merge origin/main

```

### 7. Get specific files/folder from another branch—
```
1. git checkout branch name => Go to that branch where you to add the code 
2. Git fetch origin branch-name =>  from where we want the code
3. Git checkout --patch origin dn-dev ./components/moleculs/press/   —— get the code form the press folder 
4. Check the code and do y or n
```



### 7. `Add another  remote repository`
  * git remote add origin ( repository HTTPS url  )  —— if origin is already exist then change origin with abc-origin
  * git remote -v 
  * Git fetch  or git fetch abc-origin

### 8. (a) `create branch locally and remotely`
   * git branch branch-name              => locally create branch
   * git push -u origin branch-name      => remotely create branch and push the code

### (b) `delete branch locally and remotely`
   * git branch -d branch-name              => locally delete branch
   * git push origin --delete branch-name   => remotely delete branch and push the code
    

