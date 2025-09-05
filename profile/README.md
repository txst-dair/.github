# Institutional Research Git Repositories 

<!--
👋
🙋‍♀️ Descript the organization
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

## Overview of Git

Git is a way for us to securely keep our files organized.  It has a process to keep track of each version of a file as we make changes over time.  This allows us to see and/or go back to how a file looked in a previous version if we need to. We no longer have to do manual backups of files from our share drive to make sure we don't lose our files.  We are in control of previous versions of our files and don't have to get ITAC involved to restore a file etc.

Git is not the same as GitHub (where git.txstate.edu is hosted). Git is the open source software that manages our source code. GitHub is a company (now owned by Microsoft) that hosts Git repositories and wraps it in a nice web UI, and sells software for enterprise use that provides the same service in isolated settings (as in the case of git.txstate.edu). They are not related to each other. Different people but they are often glommed together as if they are the same thing.

The naming of Git is a bit loose but it's generally not an acronym so it's rarely in all caps. The original author, Linus Torvalds, is the same guy who started and maintains the Linux kernel, and he likes to claim it was named after himself (git: slang for an unpleasant person)"

The "avpir-dev" is our Institutional Research organization ID.  All of our functional repositories should be created under this organization on git.txstate.edu.

The initital set of repositories were created (on 3/29/2023) to mimic our share drive folder structure. Although, most are empty and are just placeholders until such time the person chosen as being responsible will verify which files from the share drive are worthy of being kept and they work with me (Scott) or Kate to get the repos setup before everyone starts "cloning" them down to their harddrives. We should have a repository for each functional area in which we work to help keep things organized.

## How to install TortoiseGit tool to allow working with Git repositories

First, you'll need a way to work with Git and the Logi team showed us that they use TortoiseGit extension in Windows File Explorer.  There are other tools available to allow you to interact with a Git repository but this text only describes TortoiseGit. For a Windows setup you'll need to download and install the TortoiseGit File Explorer Extension on your Windows PC from here: https://tortoisegit.org. Just take the defaults as you go through the install wizard. If the install wizard doesn't find a "git.exe" then you'll be prompted in the first-run dialog to get it. They have a suggested website to download it here: https://gitforwindows.org/. If needed, download the git.exe and install it and take the defaults through it's install wizard. You'll be asked to enter a user name and email address (I used "Scott Henry" and my dsh17@txstaste.edu email for my setup).

## First time steps only needing to be done before you "clone" the first repository to your local harddrive: 

1. Create a folder on your local drive to hold all your IR repositories.  For example, I created C:\Users\dsh17\Documents\Git-Repos which is not a repository but will be the place I clone all repositories into. You can name your folder whatever you want. You do not need to create subfolders first for each new repo that you want to clone. The "Get Clone..." process (explained later) will create the folder for you within this "Git-Repos" folder.

## Here are the steps you'll need to do once each time you clone a new repository to your local harddrive:

1. Go to https://git.txstate.edu and log in with your Net ID and password. You won't see any AVPIR-DEV or any repositories on your first time.  But once you log in then talk to me or Kate and we'll be able to find your Net ID and add you to the AVPIR-DEV organization and give you access to all repositories. 

2. Once you can see the AVPIR-DEV organization on the git.txstate.edu website and it's repos, click on the desired repo (for example "Data-Sources-and-Repository") and there will be a URL that you need to copy (look for a "Quick Setup" area or it may be in a green "Code" Button that you'll need to click on to see the URL if you're in a repository view). We'll use this URL back in Windows File Explorer using TortoiseGit to clone the repo. There is a manual on the TortoiseGit.org website to help you figure things out: Here is how to clone: https://tortoisegit.org/docs/tortoisegit/tgit-dug-clone.html.

3. Go to your Windows repo folder (for example to (e.g. C:\Users\dsh17\Documents\Git-Repos) and right-click the folder name and select "Git Clone..." from the context menu.  Now, copy the URL into the "URL:" field.  Make sure the "Directory:" field has the folder you right-clicked (it should). Click the OK button and you may be asked to login into Git in which case select the login with browser option and use your Net ID and Password which should be prompted via your browser.  Once you log in then you will see the "Get Clone..." dialog start downloading (i.e. cloning) the repo to your local folder where it adds a folder with the name of the repo.  

## What Do We Do With Files on the Share Drive?

Once we move files from our share drive to a Git repository then we should not keep the files on the share drive.  Or, perhaps rename the share drive folder to indicate "FolderName_IN_GIT_NOW_DNU" (or something like that) so we all know not to update the file on the sharedrive but to sync up with the Git repository and work on the files on our local harddrives and then go through the process of "pushing" our local changes back up to the master "repository" on GitHub after we make updates (this process will be explained in more detail later). 

## How to Use Git
### How to see list of all Repositories while on https://git.txstate.edu/avpir-dev
You can always go back to the "top" view to see all the repositories once you're logged into GitHub by clicking on the "avpir-dev" in upper left of your browser.  The default sort for the list of repositories is by last changed but there is a SORT button that allows you to sort by other things like Name.  However, if you navigagte away and back again it reverts to the default sort by last changed.

### How to "pull" down latest files on local repository (on your harddrive)
Right-click a repository folder on your local harddrive and select "TortoiseGit" menu which will open another menu where you click the "Pull..." menu item. On the dialog that displays it will show "origin" (i.e. the name of the master repository on GitHub) and a Remote Branch of "main".  You don't need to change anything and can just click the "OK" button and it will refresh your local drive with any updated files. You should always "pull" (i.e. sync up) with the "main" repo from GitHub to update our local cloned repos to have the latest and greatest versions of all the files before you start updating a file.  However, if you forget and update an "old" file there are ways to fix it later (discussed later).

### How to "push" my files up to the "main" repo on GitHub once I'm done updating and testing it?
You can just "push" 1 file or all files.  To push 1 file just right-click it and select "Git Commit -> 'main'..." menu item. Or right-click the your local repo folder and select "Git Commit -> 'main'..." and this will display a dialog with a list of all files you've modified on your local repo in the bottom pane. You can check or uncheck which files you want to commit.  The cursor defaults to be in the "Message" free-form text box in the upper pane.  It is required to enter text in the "Message" text box to enable the "Commit" button. It is highly encouraged to always enter a description of what/why you made the change.  Add any related JIRA number or anything that would help you or someone else understand what the change was about. 

The quickest way to Commit and Push at the same time is to click the arrow on the "Commit" button and select the "Commit & Push" menu item and this will do all the steps for you instead of doing commit and push manually in separate steps. Once you do this then the button changes to be "Commit & Push" by default. You can always go back to just "Commit" if you want however it is more clicks and you may forget and only do a Commit and not a Push which doesn't push your files up to GitHub.

Here is the way to commit and push if you just click the "Commit" button which just "Stages" it on your local repo as files you have completed and want to push. On the dialog that appears after you click "Commit" you'll see messages about how many files changed and inserted but there is one more step you need to do and that is click the "Push..." button on the bottom left of this dialog. Once you click the "Push..." button another dialog appears with "Local": showing "main" and "Remote:" showing "main" and the Destination will be pointing to the Remote "origin" (i.e. the repo's name up on GitHub). You don't need to change anything on this dialog and can click the "OK" button and this will actually update the repo on GitHub. Your red circle icon with exclamation mark may not change to green circle with a check mark because Windows doesn't always refresh itself by default but sometimes it does.  You can click on another folder and then back onto the folder with the file(s) you just checked in you'll they all have the green icon now.  

### What are the new icons on my folders in File Explore?
TortoiseGit extension adds these colored icons to help you see what is up-to-date/changed on your local repo.  You'll see a green circle with a white checkmark if your local repo has been refreshed.  The top folder will stay green even if you have changed files deeper in the folder structure of your local repo. If you do a "pull" request on a green circle with a checkmark repo you'll even be told "Already up to date" in that Pull dialog discussed earlier.  You'll see a red circle icon with an exclamation mark on files you have changed since your last Pull.  These colored icons do not show differences as compared to the source in the "origin/main" repo up on GitHub.  When you try to commit changes you'll be notified that there are conflicts and this will be explained later.

### How do I see what changes I have made?
Right-click a file you have changed and select "TortoiseGit" menu item and then select the "Diff" menu item. I dialog will appear showing a side-by-side view of what you have changed on the right side and what the source looked like when you pulled down the "main" on the left side. You can even make changes to your local version (right side) in this dialog. In the toolbar there are options like "Next difference" and "Previous difference" to help you navigate to each difference in the code.  

To see all files you have changed in your local repo you can click to repos top folder and select "TortoiseGit -> Diff" and it will show you a list of all files you have changed locally.

### What happens if another person has updated a file I want to make changes to?
If 2 or more people are working on the same file and they pushed a file up to GitHub since you last sync'd up then there will be a conflict that must be resolved in your code before you can "push" it up.  You won't see this conflict until you try to commit/push your changes.  After you click the "Commit & Push" button you see an error in red in a log that will look like the following:

*"git.exe push --progress "origin" main:main  
To https://git.txstate.edu/avpir-dev/data-repository.git  
! [rejected]        main -> main (fetch first)  
error: failed to push some refs to 'https://git.txstate.edu/avpir-dev/data-repository.git'  
hint: Updates were rejected because the remote contains work that you do  
hint: not have locally. This is usually caused by another repository pushing  
hint: to the same ref. You may want to first integrate the remote changes  
hint: (e.g., 'git pull ...') before pushing again  
hint: See the 'Note about fast-forwards' in 'git push --help' for details  
git did not exit cleanly (exit code 1) (813 ms @ 3/30/2023 11:14:24 AM)"*  

To resolve this conflict you'll need to patch your local code to include the code that someone else checked it (if it makes sense still).  We're a small team so you can always go talk to the other person and decide who the file should be changed to resolve the conflict.  You resolve by first clicking the "Pull..." button on the bottom left down below the error log dialog. Another dialog appears where you can click "OK". It will attempt to merge the file for you but if you happen to have changed the same line(s) of code then another error will display:

*"While merging, i.e. integrating changes of another (remote) branch into your local branch, a conflict in at least one file occurred. This means that you need to resolve this manually (i.e. you need to integrate your changes into a file which was also modified on another branch). After resolving all files, you need to perform a commit in order to complete the merge. If you want to abort the merge , do a hard reset on HEAD or select abort merge on the context menu.  See help for more information."*

Click the "OK" button on this new error dialog. Now back in Windows File Explorer you'll a new icon on your file which is a yellow triangle with an exclamation mark in it indicating it needs to be resolved. The original "Commit & Push" dialog has changed now to have a "Resolve" button in the bottom left where the "Pull..." button used to be. You can resolve these conflicts in multiple ways. You can click the "Resolve" button on this dialog or back in Windows File Explorer you can right click the file with yellow triangle icon and select "TortoiseGit > Resolve..." or you can click the "Edit conflicts" menu item or you can click "Abort merge" if you just want to stop and start over. 

I prefer clicking the "Edit conflicts" context menu item because that brings up a side by side view of the differences and it allows you to keep one or the other of the changes on the same line or keep both. There is are toolbar options called "Use left text block" and the "Next conflict" and "Previous conflict".  The dialog doesn't go to the first conflict by default so I use click the "Previous different" toolbar button to go to the top most difference and then if it is a conflicting line then "Use left text block" toolbar option will now be enabled. If it is not the first conflicting line then use the "Next conflict" toolbar button to go to it.  The "Use left text block" button has an down arrow on it that, when clicked, shows additional options of "Use right text block", "Use left text block then right", and "Use right text block then left". These are all ways you can pick and choose which line of text you want to keep. Once you make your selections the pane on the bottom will show the changes as you have directed it to do.  Once you have resolved all conflicts (you won't see any red lines anymore) and you are satisified with the lower pane version of your file you can click the "Mark as resolved" button in the toolbar and then click the "Save" button in the toolbar and close the dialog. Your file's icon should now be green with a checkmark. You still need to do testing of your code (SQL) and then "Commit & Push" to get your code up to main repo.

When you enter the "Commit & Push" dialog a message will be displayed telling you:

*"The commit you are composing is a special commit. It is a merge commit and, thus contains your changes as well as the changes of a merged branch. You shoult NOT uncheck files unless you know what you are doing. When you merge changes, conflicts can arise that must be solved manually (i.e., you need to integrate your changes into a file which was also modified on another branch). See help for more information."*

You can just click the "OK" button or before doing that you can click the check box "Don't show this message again" as this is just telling you that it is a special commit with a merge.  Now you can click the "Commit & Push" button and you'll be presented another message dialog stating:

*"It looks as if there is a conflict hint (a line like "# Conflicts") in your commit message. This hint is automatically added by Git for cli users and there is no need to keep it. Do you want to ignore this warning and keep these lines or abort committing in order to edit the commit message? You can automatically remove these lines by enabling 'Strip lines starting with '#' in commit messages' in TortoiseGit settings."*

You can keep the conflicts text in the message if you want to you remember you had to do a merge with someone elses code. Or you can Abort and edit the message to remove the # Conflicts lines if you want to. And you can click the check box "Don't show this message again" and never have to deal with it ever again.

This conflict resolution doc applies to text files.  Binary files like Word, Excel, etc., will be different. In fact we may decide to just keep Word, Excel docs in Teams perhaps... still thinking on these types of files...

## This README file will be updated in the future with more detail on how to use Git... 

... to be continued...
