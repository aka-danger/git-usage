# Git workflow

NOTE: steps starting from when you start developing

##### STEP 1:
- `git clone`           -> add repo to your computer. if you have cloned then move to STEP 2
- `git checkout master` -> go to the master branch
- `git pull`            -> Get the latest version of the master branch from the Remote to local 
- `git checkout <your branch>` -> go to your branch 
- `git merge master`    -> make sure your branch is inline with the master. if you get alot of merge conficts it means your branch is not upto date with the master and you either need to clone again or you need to resolve the confilcts and follow STEP 2

##### STEP 2:
by now you have been programming for a while so you must commit your changes (in your branch) and do these steps (**before pushing**)
- `git commit`          -> commit changes
- `git checkout master` -> switch to master
- `git pull`            -> Check if there are no new changes in the master since you have been devloping, someone else might have made changes
- `git checkout <your branch>` -> switch back to your branch
- `git merge master`    -> when in your branch try to merge your branch with the master. if you get conficts you need to fix them ([Resolving conflicts](https://www.youtube.com/watch?v=zz7NuSCH6II)).if it says already-up-to-date or merges your changes then it means that your changes are fine and you can move to STEP 3
- `git push`            -> push your changes and go see on github if they are all good. you will probably get notification to **compare** and **pull** on github

##### STEP 3: PULL REQUEST
once you have pushed
- got to your branch on github and click `new pull request`
- it will take you to a page. then wait and let it tell you if you can **merge automatically**
- if you cannot **merge automatically** then you need to go back and resolve the conflicts on your branch with the master.
- if there are no problems then you can create a pull request but do not commit the changes to the master. someone else should be reviewing your code
- the more pull requests that are made and commited to the master the more additions to the project

#### Note: 
the master is always the most up-to date version and you need to continuously make additions to it.
there is absolutly no reason that the master should be changed directly. the only way the master is changed is through a pull request.
make sure you are on your branch and only affecting your branch. note also that these are the only collaberative command that you need to use



