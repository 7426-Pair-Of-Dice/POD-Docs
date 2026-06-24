# Branching with the Terminal
In this tutorial, you will be shown how to use branches with the Git Terminal.

- [Creating Branches](#creating-a-branch)
- [Deleting Branches](#deleting-a-branch)
- [Deleting Remote Branches](#deleting-remote-branches)

## Creating a Branch:
1. Make sure that you are **on** the main branch before following this tutorial. If you are not sure that you are on the main branch, look at your bottom left corner in VSCode! It should say main, like in the example below!  
![Check](../img/gitimgs/BranchCheck.png)  
If you are **not** on the main branch, click on that button and switch to the **main** branch!
![MainBranch](../img/gitimgs/SwitchToMain.png)

2. To start, create a new terminal in VSCode!
![Terminal](../img/gitimgs/TerminalCreation.png)

3. Type in this command:  
**git switch -c "[branch-name]"**  
This command will create a local branch that you can use to work! That's great, but we want to publish it to the cloud so that we can use it if things go wrong.

4. Type in this command:  
**git push -u origin "[branch-name]"**
This command will create a remote branch that will be saved to Github!

    Once you have entered this command, you have successfully created a remote branch!   
    As always, if you ever need any help, ask your programming mentors! They will guide you in the right direction!

## Deleting a Branch:
1. Make sure that you are **on** the main branch before following this tutorial. If you are not sure that you are on the main branch, look at your bottom left corner in VSCode! It should say main, like in the example below!  
![Check](../img/gitimgs/BranchCheck.png)  
If you are **not** on the main branch, click on that button and switch to the **main** branch!
![MainBranch](../img/gitimgs/SwitchToMain.png)

2. To start, create a new terminal in VSCode!
![Terminal](../img/gitimgs/TerminalCreation.png)

3. Type in this command:  
**git branch -d "[branch-name]"**  

    This command will delete your local branch!
    That's great, but we want to delete it from the cloud so that we don't confuse people with a "dead" branch.

## Deleting Remote Branches:
Remember that Github saves things to the cloud. That means that we need to get rid of the branch on the cloud as well. Remote branches can only be removed with the terminal.

1. To start, create a new terminal in VSCode!
![Terminal](../img/gitimgs/TerminalCreation.png)

2. Once you have a terminal, type this command in there:  
**git push origin --delete "[branch-name]"**  
It should look something like this:
![Delete1](../img/gitimgs/FirstDelCommand.png)  
This command will delete your branch on the cloud! Be **careful** with the branch name! Make sure that you are removing **your own** branch! Git **is** case-sensitive and it will throw errors if a branch was not found.

3. Once that has been completed, type this command in there:  
**git fetch --prune**  
This command will fetch the latest version of the repository which will not have your remote branch! Your terminal output should look similar to this if you were successful!
![Full View](../img/gitimgs/FullTerminalView.png) 

Once you have finished, you have successfully deleted your branch!   
As always, if you ever need any help, ask your programming mentors! They will guide you in the right direction!