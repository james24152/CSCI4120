Guide for setting up environment:

1. Accept the collaboration invite in email
2. Install git at https://git-scm.com/downloads
3. Install git lfs at https://git-lfs.github.com/
4. After installing git, you will be able to open `git bash` , we will use that to insert command and do version control.
5. Install GitHub Desktop at https://desktop.github.com/
6. Open GitHub Desktop and sign in
7. Go to `File` -> `Clone Repository` -> Enter the CSCI4120 repo URL -> Clone the repository at your desired location
7.1. If there is a prompt asking you to set up lfs, then say yes
8. Open the Unreal project without closing GitHub desktop and git bash
9. The map is at `Medieval Dungeon` -> `Map` -> `Demostration`
10. Before doing any modifications, Press `Source Control` at the top and link a source control
11. Select `Git`, then find git.exe(which you have installed in step 2) and select it as the path
12. If there is an option to activate lfs, then be sure to tick it.
13. Press Accept settings and a prompt at the bottom right will notify you that the connection with git is established
14. Go back to GitHub desktop, if you are not prompt to activate lfs, then in Git Bash, go to the directory where you clone the files
(you will see Master at the end of the path if you did it right), and type `git lfs install`
15. Now you are all set and can modify files and try to push it

Guide to do simple push pull:
1. Make sure you finish every step stated above
2. Try modify something in the `Demostration` map, after that you may see a ? on the modified file in the `Content Browser`
If this happens that means you successfully connected the project to Github
3. Save all the files then open Git Bash
4. Always change directory to the path where you cloned the project. This is where you will execute git commands
5. Type `git status` to see what files you have modified (They appear in red color)
6. Type `git add .` to add the files for commit (The . means all the modified files)
7. Type `git status` again to see what files are being added (Added files appear in green)
8. Type `git commit -m "abcdefg"` to commit the files changes
Commiting means you are sure you want to change the files and the commit message notify others what is changed by you 
(Replace the "abcdefg" to whatever you want)
9. Type `git push origin master` to push the changes to the remote repository and let everyone know about the changes
10. Type `git pull` to update your local repository so that you can see what changes are made by others

**Important Note:
Every file in the unreal project, including .uasset and .umap, CANNOT BE MERGED. Therefore, WE NEED TO SET UP A DEVELOPMENT SCHEDULE
TO ENSURE WE DO NOT DEVELOP AT THE SAME TIME. DO NOT TRY TO STASH APPLY ANY FILES OR THINGS WILL TURN TO SHIT. Thanks.**
