### Answer the following questions in you own words.

> It's not necessary that you havee to know and answer all the questions. Just answer the ones
> you know and write in your own words.

1. Give the difference between the remotes - upstream and origin - with an example.

You answer: origin means my copy of a repository which i fork and clone and when i make any changes i i push and pull from origin whereas upstream is used to get the update or any other feature that is added in my repository from the original repository which i fork and clone.

2. You have two branches A and B and you have currently made some changes in branch A.
You want to move into branch B but do not want to commit the current changes in branch A.
What will you do?

You answer:I will use the git stash command which helps me to save any work which i dont want to commit and then it changes to the last commit then i can switch branch and do the other work and then again return to the the previous branch and do the unfinished work and commit it.

3. You were assigned a work to implement a feature and create a PR to your organization's remote repository.
For this you made a branch (say A) and made some changes and commited them. Now you moved to some other branch 
(say B) to do some other assigned work. But later you realisd that have to complete the task assigned earlier 
first and commited some changes in branch B which are meant for branch A. How will you use git to bring the 
changes from branch B to branch A?

You answer:I wil use git rebase command .first i will switch to branch b using git switch b and use git rebase a which adds the commits of b on the top of the latest commits of a. then i will move to the branch a and merge branch a and b and then i will remove the commits from b.

3. What is the difference between fetching changes and pulling changes?

Your answer:fetching changes means updates the latest commits from the original repository to my local repository, but does not changes current branch whereas in pulling changes it does all the things that fetching does but it also changes the current branch but in fetching we have to manually merge the changes into my branch.

4. What does -i flag stand for? What is it's significance in git?

You answer:-i flag means interactive.it is mainly used with rebase. it allows to interactively change commits.it helps us to reorder combine edit delete commits.

5. You are working in an organization that follows very strict guidelines for PRs and commits.
You made three commits in your PR and the maintainer says you were supposed to make a single commit.
What will you do in this case?

You answer:i will use the git reset --soft HEAD~3 command which will take me 3 commits back and now i will make a new single commit with all those changes.

6. Explain `git merge` and `git rebase` with example(s).

You answer:gi merge combines changes from one branch to another branch. it keeps the full history of both the branches while git rebase makes the commit looks linear like the another branch was started from the main branch only.

7. Write the flow how you create a repository and push changes to it. Also mention the commands used at each step.

You answer: Create a repository on github.
first initialise git in your project folder by using command git init
then add all the files by using command git add .
then commit the changes using command git commit -m "Your message"
now connect your project folder to the repository you made using command 
git remote add origin https://github.com/username/repo.git
now push changes to the repository using command git push -u origin main

8. How would you prevent a file or folder from getting tracked by git?

Your answer:by adding that file or folder in .gitignore

9. You did not implement the step you mentioned in question 8 and now you have committed and pushed your database's
secret key to the github. How will you remove the key from your git's commit history to avoid any misuse?

You answer:i will use git reset --hard commitHash to remove it and then add that file in .gitignore then again push changes

---