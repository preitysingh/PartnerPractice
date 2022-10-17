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



`*   commit edab0a6a50fe6aa77510ea8f43f2dd5869eafb7f (HEAD -> main, origin/main, origin/HEAD)
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
|       Preity's edit 2 for txt
|
* commit 317a78ebfa61e6ab8ed73d1e762cf29df6ae3d20
| Author: Preity Singh <psingh23@kentdenver.org>
| Date:   Mon Oct 10 14:01:22 2022 -0600
|
|     adding preity's feature 2 text
|   
*   commit 5e3f965ab17abfc43ce5590dcc4d68229f9f9a9b
|\  Merge: aefb308 6225300
| | Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
| | Date:   Mon Oct 10 13:55:54 2022 -0600
| |
| |     Merge pull request #1 from preitysingh/lilly
| |     
| |     Lilly
| |   
| *   commit 6225300f9ec7b5b4ceb771262e0a41de724a9ae3
| |\  Merge: 5ee5745 e792e4a
| | | Author: lillyphan <lphan24@kentdenver.org>
| | | Date:   Fri Oct 7 10:49:11 2022 -0600
| | |
| | |     Merge branch 'main' of https://github.com/preitysingh/PartnerPractice into lilly
| | |     
| | |     Merge main and feature.
| | |
| * | commit 5ee574516b90d0ebb2aadc7104d2704b4826fa57
| | | Author: lillyphan <lphan24@kentdenver.org>
| | | Date:   Fri Oct 7 10:39:13 2022 -0600
| | |
| | |     Add and edit otherfile.txt
| | |
* | | commit aefb308bb2543d676b56a61be67f3fa65b87b8d3
| | | Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
| | | Date:   Mon Oct 10 13:50:25 2022 -0600
| | |
| | |     Update README.md
| | |
* | | commit b9f12bd1fd6813805a884a2c488d55feb814750d
| | | Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
| | | Date:   Mon Oct 10 13:43:13 2022 -0600
| | |
| | |     Update README.md
| | |
* | | commit a0d542b374f56e1acd5e82f3ee9d861c93390a33
| | | Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
| | | Date:   Fri Oct 7 13:24:08 2022 -0600
| | |
| | |     Update README.md
| | |
* | | commit 2db03c2a23b6e77c236a8415ca7a6880545f1319
| |/  Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
|/|   Date:   Fri Oct 7 11:01:15 2022 -0600
| |   
| |       Update README.md
| |
* | commit e792e4a3e99ca2ff150695a44360aa560fb445ab
|/  Author: Preity Singh <psingh23@kentdenver.org>
|   Date:   Fri Oct 7 10:30:34 2022 -0600
|   
|       Tired message
|
* commit 016a252c1994178e2ef0f7520ff6fbaf7811def9
| Author: Preity Singh <psingh23@kentdenver.org>
| Date:   Fri Oct 7 10:24:45 2022 -0600
|
|     Add Text File
|
* commit b186848d894b046558398786aa6b40cbf2281deb
| Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
| Date:   Fri Oct 7 10:20:09 2022 -0600
|
|     Update README.md
|
* commit 99ca93855478d98716c8faed033383ae60a40efc
  Author: preitysingh <111521777+preitysingh@users.noreply.github.com>
  Date:   Fri Oct 7 10:17:59 2022 -0600

      Initial commit`
