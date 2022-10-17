# PartnerPractice

Q1 - What does clone set the variable origin to represent?
**-->The clone sets "origin" to the local repository**

Q2 - What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?
**--> pushes commits from local repo (origin) to main (remote repo)**
**--> in this context, remote tracking means that when you use --set-upstream, git will be able to track the local repo and remote repo referenced in the command together. this means that in the future when you use git pull, push, or fetch, git will assume that you want to call those in reference to that pair of repositories**

Q3 - Explain and illustrate what's happening in the commit tree when this command executes.
**--> git pull origin master pulls changes from the remote main branch and merges them to the local check-out branch, visually, it combines the histories of the remote and local repos, (one line!)**

Q4 - Are your commits overwritten by the remote master?
**--> no, commits were not overwritten**

Q5 - Is this a merge or a rebase?
**--> this is a merge**

Q6 - Person B: checkout the local master branch. Is it updated as well, or still behind remote master?
**--> ???????**

Q7 - Run git branch. Did your local copy of your branch delete when Person A deleted the remote branch? If not, delete the local copy of the branch using git branch -d BRANCHNAME
**--> no, the local copy of the branch did not get deleted, deleted branch**

Q8 - Use git log --graph --all to view the branching structure and copy and paste the result into the README.md formatted as a code segment (see markdown cheatsheet).

*   commit edab0a6a50fe6aa77510ea8f43f2dd5869eafb7f (HEAD -> main, origin/main, origin/HEAD)
|\  Merge: 61474b3 5ef4303
| | Author: lillyphan <113716236+lillyphan@users.noreply.github.com>
| | Date:   Tue Oct 11 11:07:53 2022 -0600
| |
| |     Merge pull request #2 from preitysingh/feature2
| |     
| |     Feature2
| |   
| *   commit 5ef430336ab8e5286b95c0993c9f9539f81cc243
| |\  Merge: 9f0439f 61474b3
| |/  Author: lillyphan <113716236+lillyphan@users.noreply.github.com>
|/|   Date:   Tue Oct 11 11:07:46 2022 -0600
| |   
| |       Merge branch 'main' into feature2
| |
* | commit 61474b39d16e125a7ef5578d639bb565fdd1080b
| | Author: lillyphan <lphan24@kentdenver.org>
| | Date:   Mon Oct 10 14:07:12 2022 -0600
| |
| |     Edit text2.rtf
| |   
| *   commit 9f0439f92e8620f5745ceeceb11b705d7453770b
| |\  Merge: 60bc014 ddbb066
| | | Author: Preity Singh <psingh23@kentdenver.org>
| | | Date:   Tue Oct 11 11:03:56 2022 -0600
| | |
| | |     fix conflict
| | |
| | * commit ddbb066b0dc9517b49f8d17532a2ccda826d6d8f (feature2)
| |/  Author: lillyphan <lphan24@kentdenver.org>
|/|   Date:   Mon Oct 10 14:16:15 2022 -0600
| |   
| |       Lilly
| |
| * commit 60bc014d47435097f26027f63f1897e28c972e10
|/  Author: Preity Singh <psingh23@kentdenver.org>
|   Date:   Mon Oct 10 14:16:28 2022 -0600
|   
:
