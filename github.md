## Git  commands 
### 1.  `Get specific files/folder from another branch—`

  * Git fetch origin branch(remote branch) name ———  where we want the code 
  * Git checkout --patch origin/dn-dev ./components/moleculs/press/   —— get the code form the press folder 
  * Check the code and do y or n

  
### 2. `Merge —`
  * git pull origin mein  —— merging code from main branch
  * Git pull —— merging code from current branch only
    
### 3. `Revert — ( remove its changes from our branch )`
  * git revert {commit_id} — Sometimes we want to undo a whole commit with all changes
  * git push origin +{commit_id}^:master ——  Delete the last commit
    
### 4. `Add another  remote repository`
  * git remote add origin ( repository HTTPS url  )  —— if origin is already exist then change origin with abc-origin
  * git remote -v 
  * Git fetch  or git fetch abc-origin
    
### 5. `Specific commit using cherry pick.`   —— Cherry picking is the act of picking a commit from a branch and applying it to another
  * git cherry-pick <COMMIT HASH> . git add . 	

