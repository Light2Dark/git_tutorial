# Git and Github Tutorial

#### This branch is a testing branch for how you would want to work with branches in a team. Since git pull only fetches and merges the main branch of a repository, you need more commands to pull a branch into your local repo.

## Steps
0. Let's say in GitHub there is a new branch created by a team member called <b>develop</b>
1. In your own machine, type:
```bash
git switch develop
```

## Behind The Scenes Steps (imagine you didn't do git switch)
0. Let's say in GitHub there is a new branch created by a team member called <b>develop</b>
1. Create a new branch in your local repo (I'll name it waffles)
2. Switch to that branch
3. If you do a git pull, you will get an error saying that this branch does not know where to pull from so..

```bash
git branch --set-upstream-to=origin/develop waffles
git pull
  OR
git pull origin develop
```

4. The command above basically tells the branch where to pull from, and we will specify that we want this branch to pull
from the develop branch in origin
5. Now you're done and you can work on this branch with your teammate!
6. Remember to pull before pushing
