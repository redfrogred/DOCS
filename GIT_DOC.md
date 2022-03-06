# GIT IN 10 COMMANDS (OR LESS)

I firmly believe that you can git by with knowing only 2% -- 
            or even less! -- of almost anything.  If you
            know the right 100 words in Spanish, you can travel in Spain just fine.  And if you
            know the right 5-10 git commands, you can do just fine with GIT.

Here are those 5-10 commands:  

 
> git clone GIT_REPO_URL  

and

> git status  
> git add .  
> git commit -m "blah blah blah"  
> git push origin BRANCH_NAME  

These next few are a level below...

> git checkout BRANCH_NAME  
> git checkout -b "BRANCH_NAME"   
> git pull  

Finally, there are these less-used ones:

> git reset (undo "add" for all added files)  
> git branch -a (This shows all branches)  
> git reset --soft HEAD^ (removes last local commit)  
  
  
___  
___  
___  

_IF YOU NEED TO DELETE A BRANCH_ (and restore things locally, to how they were before a failed branch effort) do this:

> git checkout main  
> git fetch origin  
> git reset --hard origin/main 
> git clean -f -d 

^ from https://stackoverflow.com/questions/42877852/undo-local-changes-in-git (see answer from "Stevoisiak")
