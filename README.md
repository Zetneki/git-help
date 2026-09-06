[Git cheat sheet](https://git-scm.com/cheat-sheet)  

git push -u `<repository>` `<name>` 
  - -u links your local branch to the given remote branch  
  - `<repository>` is the remote repository name  
  - `<name>` is the given name to the branch  

git init -> start a new repo  
git remote add "origin" git@github.com:User/UserRepo.git -> add a new remote  
git remote set-url "origin" git@github.com:User/UserRepo.git -> change the url of an existing remote repository  
git add . -> add all untracked files and unstaged changes  
git commit (--amend) -m "message" -> make a commit (change a commit message or add a file you forgot)  
git rm (--cached) `<file>` -> delete file (tell Git to forget about a file without deleting it)  
git restore -> delete unstaged changes to one file  
git checkout `<id>` -> switch to a different commit state  
git pull (origin `<branch name>`) -> fetch changes and then merge them into your current branch  
git push (origin `<branch name>`) -> push the given branch to the remote origin  
git switch -c -> create a branch and switch to it  
git switch -> switch branches  
git branch -> lists the branch names  
git branch -d `<name>` -> deletes the given branch  
git status -> check the current state of your working tree  
git log --all --graph -> look at the commit history of all branches  
git fetch -> fetch changes (but don't change any of your local branches)  
git rebase `<name>` -> replay the current branch's commits on top of `<name>`  
git merge `<name>` -> merge the `<name>` branch into the current branch  

If the main branch is ahead of another branch, first merge main into that branch, then later merge the branch into main.  

In case of a merge conflict, choose either one of the changes or create a completely new solution in all of the affected files.  
Then mark the conflicts as resolved (git add) and commit the merge.  
Git keeps the version you resolved the conflict with.  
