# PartnerPractice

Q1 - What does clone set the variable origin to represent? 
**-->local repo**

Q2 - What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?
**--> pushes merge commits to the remote repo**
**--> remote-tracking branches are *references* to the state of remote branches**

Q3 - Explain and illustrate what's happening in the commit tree when this command executes.
**--> git pull origin master pulls changes from the origin remote, master branch and merge them to the local check-out branch**

Q4 - Are your commits overwritten by the remote master?
**--> 

Q5 - Is this a merge or a rebase?

Q6 - Person B: checkout the local master branch. Is it updated as well, or still behind remote master?

Q7 - Run git branch. Did your local copy of your branch delete when Person A deleted the remote branch? If not, delete the local copy of the branch using git branch -d BRANCHNAME

Q8 - Use git log --graph --all to view the branching structure and copy and paste the result into the README.md formatted as a code segment (see markdown cheatsheet).


