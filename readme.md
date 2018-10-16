# IH_Project1
## Resolving Merge Conflicts

1. From the user folder, a directory called "IH_Project1" is created using the **mkdir** command
2. Navigate to the recently created directory using **cd ~/IH_Project1**
3. The **git init** command is executed to create the local repository. To check that the repository was correctly created, the command **ls -a** needs to be run to allow checking on the existance of the **.git** file.
4. The command **nano readme.txt** is used to create a new text file called readme.txt whose content must be modified to read an example of text.
5. Another file named "uniqueiteminmaster.txt" is created using the same method as in the previous point.
6. Once the files are created, the command **git add** is used to allow git to track changes on them.
7. In Github, a new remote repository must be created and associated with the local repository by adding the two lines of code specified in the remote repository's code tab.
8. In order to communicate the changes to git, the command **git commit -am** is run. The command **git status** will now reflect that git is up to date and therefore, it is time to run the **git push** in order to update the remote repository with the local updates.
9. A new branch names "Colaborador" is now created by using the command **git checkout -b Colaborador**. When trying to push the new branch, an error prompts informing of the unability to communicate with the remote repository. The line **git push --set-upstream origin Colaborador** must be used to solve the issue.
10. From the Colaborador branch, the content of the readme.txt file is modified, adding miscellaneous information in the odd lines and always adding the sentence "belongs to master branch" in the the even lines. Once modified, the file is saved.
11. Once modified, the command **git status** is used to check the current sync status of the files. The command **git commit -am** is used to update the local repository with the latest changes
12. The process of modification, status and commit is repeated a few times to observe different milestones in the github network diagram
13. Once several commits are completed, it is necessary to run **git push** from the Colaborador branch in order to update the remote repository with the local updates.
13. Back in the local repository, the code **git checkout master** is used to change the working branch.
14. The readme.txt is open from this branch, showing as it was originally. The content is modified adding miscellaneous information in the even lines and the reference "belongs to Colaborador branch" in the odd lines. Note that this is the opposite as in point 10 in order to generate a conflict.
15. The process of modification, status and commit is repeated a few times to observe different milestones in the github network diagram
16. Once several commits are completed, it is necessary to run **git push** from the master branch in order to update the remote repository with the local updates.
17. From the master branch, merge the branches using the command **git merge Colaborador**
18. An error message will prompt informing of the conflict in the readme.txt. The command **cat readme.txt** is used to show a comparison between the two readme.txt versions that are causing the conflict.
19. Visual Studio Code should be used to modify the content of the readme.txt file in order to set the final version. Once the readme.txt is saved, the conflict will be solved and the branch merged.
20. Run the command **git commit -am** to update the local repository
21. Run the command **git push** to communicate the latest changes to the remote repository.

![NetworkDiagram](AlbertoCastellanos.github.com/IH_Project1/NetworkDiagram.png)


