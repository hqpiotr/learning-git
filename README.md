# learning-git based on Pro Git book!
Latest page read: 

### git add: 
    - treat as "add precisely to the commit next time",
    - not the "add new files only"
    - If  you  modify  a  file  after  you  run  git add,  
    - you  have  to  run  git add  again  to  stage  the latest version of the file!
### git diff:
    - It’s  important  to  note  that  git  diff  by  itself  
    - doesn’t  show  all  changes  made  since  your  last commit
    - only  changes  that  are  still  unstaged.  
    - If  you’ve  staged  all  of  your  changes,  
    - git diff  will give you no output.
### git log:
    - git log -p 
        // patch - pokazuje zmiany
    - git log --stat 
        // statystyka dodan/usuniec
    - git log --pretty=format:"%h: %an, %ar, %s"
    - git log --oneline 
    - git log --since=2.weeks
    - git log --since="2 years 5 months 3 days ago"
    - git log --author="Piotr" --oneline --grep="remove"
    - git log --pretty="%h - %s" --author='Junio C Hamano' --since="2008-10-01" --before="2008-11-01" --no-merges -- tests/
        // find commits which are not merges from specific author done in specific month under the tests subfolder.

### git commit 
    git commit --amend:
        // The  obvious  value  to  amending  commits  is  to  
        // make  minor  improvements  to  your last  commit,  
        // without  cluttering  your  repository  history  with  
        // commit  messages  of the form, “Oops, forgot to add
        // a file” or “Darn, fixing a typo in last commit”.

### git reset 
    - git reset HEAD some_file.txt:
        // unstage staged file
        // new cmd from git 2.23 is: git restore ! NEW COMMAND !
### git restore
    - git restore --staged STAGED_FILE.txt
        // remove the staged file from stage

    - git restore MODIFIED_FILE.txt
        // unmodify the modified file
    -git checkout -- MODIFIED_FILE.txt
        // discard/undo the changes that you made to the file
        // go back with the code. !!! DANGEROUS! You stashing instead!

### git remotes
     - git remote 
        // to show what pointers you have // origin
     - git remote -v 
        // to show full paths https
     - git remote add acronym https://....
     - git fetch <origin>
     - git remote show origin 
        // shows https address.
     - 

