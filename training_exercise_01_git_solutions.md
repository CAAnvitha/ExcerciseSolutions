# Description: Git Exercise

### 1. List the Global Configs
* List the git global configs
```
git config --list 
```

### 2. Track a New Project With Git
* Create a sample project in a dir

```buildoutcfg
mkdir ExcerciseSolutions
cd ExcerciseSolutions
```
* Track the above project with git
```
git init
```
* Identify the location of config for the project
```buildoutcfg
/home/anvithaca/Desktop/training/ExcerciseSolutions/.git/config
```


### 3. Stage a Changed File 
* Modify an existing file
```buildoutcfg
cat Readme.md
```
* Add a new file to the project
```buildoutcfg
touch git_exercise.txt
git add README.md
```
* Stage the file changes
```buildoutcfg
git commit -m "Added changes in readme file"
```

### 4. Revert the Staged Files
* Modify an existing file
```buildoutcfg
cat git_exercise.txt
```
* Add a new file to the project
```buildoutcfg
touch new.txt
```
* Stage the file changes
```buildoutcfg
git add new.txt
git commit -m " Added new.txt file"
```
* Revert the staged files
```buildoutcfg
git reset --HAR
```

### 5. Commit all Unstaged and Staged Files at Once
* Add a new file
```
cat > aboutme.txt

```
* Stage the file change
```buildoutcfg
git add aboutme.txt
git commit -m "Added aboutme.txt
```
* Modify an exiting file
```buildoutcfg
cat aboutme.txt
```
* Commit all the changes at once
```buildoutcfg
git add *
git commit -m "Added all changes"
```

### 6. Commit Selective Files
* Add 2 new files
```buildoutcfg
cat > frech.txt
cat > german.txt
```
* Modify 3 existing files
```
vi git_exercise.txt (press  'Esc' key and type :wq! to save)
vi README.md (press  'Esc' key and type :wq! to save)
vi new.txt (press  'Esc' key and type :wq! to save)

   or

('cat > filename' will overwrite the content)
('cat >> filename' will append the content  )
cat [>][>>] git_exercise.txt
cat [>][>>] README.txt
cat [>][>>] new.txt


```
* Pick 1 each from the above files and commit
```buildoutcfg
git add french.txt
git commit -m " Added french.txt"
```

### 7. Change the Previous Commit Title
* Change a file and commit

* Now modify the commit title

### 8. Modify the Title for Already Pushed Commit
* Change a file and commit
* Push the changes to remote branch
* Now modify the commit title
* Push the changes again and create a merge request
* List the problems

### 9. Delete a Local Branch

### 10. Delete a Remote Branch

### 11. Undo Last Unpushed Commit
* Create branch from develop
* Modify a file and commit
* Now undo the changes

### 12. Undo Last Pushed Commit
* Create branch from develop
* Modify a file and commit
* Push the branch to remote
* Now undo the changes

### 13. Add Missed Files to the Previous Commit
* Checkout a branch from develop
* Modify 5 files
* Commit only 3 files
* Now add the rest of 2 file changes to the same commit

### 14. Merge Conflict
* Form a team of 2 developers Dev1, Dev2
* Dev1 creates a new branch test-branch-{dev_name} from develop.
* Dev1 modifies a line in existing file, commits and pushes the branch to remote.
* Dev2 creates a new branch test-branch-{dev_name} from develop
* Dev2 modifies the same line in the same file and commit.
* Dev2 now should take the change from dev1 branch and push the dev2 branch to remote.

### 15. Cherry Pick a Commit From Other Branch
* Create a branch test-branch-1 from develop
* Modify a line in a file and commit
* Now modify the same line and commit again
* Checkout to develop branch
* Now create another branch test-branch-2 from develop
* Get the changes of first commit from the test-branch-1 to test-branch-2

### 16. Preserve the Uncommitted Work Done on Main Branch
* Checkout to develop branch and remember the state.
* Change a file and commit
* Change another file
* Work on a new task from the previous state of develop branch while preserving the previous work.

### 17. Fix a Spoiled Local Branch
* Checkout a new branch b1 from develop
* Make a file change and commit
* Checkout to develop and create new branch b2
* Change a file and commit
* Now merge b1 into b2
* Change another file and commit
* Change couple more files
* Do git add for 1 change
* Now Fix the b2 branch not to have b1 changes but rest of the changes.

### 18. Save the Committed, Uncommitted Work in a File and Get it Back.
* Checkout a new branch b1 from develop
* Change a file and commit
* Change another 2 files and run git add 1 of those files
* Now save the state to a file and restore it back in your partner's system.
