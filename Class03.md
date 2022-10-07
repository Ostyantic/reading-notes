# **Version Control(VCS) & Git**

Version control is a system that allows one to revisit various versions of a file or set of files by recording changes.
With Version control, one can:

- revert a file or project to a previous version
- track modifications and modifying individuals
- compare changes
- fix mistakes with files

## **Different Types of Version Control**

*Local Version Control* - A VCS that consists of one database on a hard disk that stores changes to files.

*Centralized Version Control(CVCS)* - A VCS that consists of a single server that stores all changes and file version that can be accessed by multiple clients.

*Distributed Version Control(DVCS)* - Does what CVCSs do, but better. This system allows clients to mirrored repositories so that in case data is lost, they can easily be backed up since there are basically multiple mirrored copies. This system also allows programmers to collaborate with each other to complete joint projects.

## What is Git?

Git is a DVCS that stores data in a file system made up of **snapshots**. Whenever a change is made and save, aka commit, Git creates a snapshot of the file and stores it for later reference.

### Local Operation

Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

### Trackin Changes

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

### Loss of Data

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

## States in Git

Files in Git can reside in three main states: **committed**, **modified** and **staged**.

### **Committed** - Data is securely stored in a local database

### **Modified** - File has been changed but not committed to the database

### **Staged** - Flagged a file’s changed version to be committed in the next snapshot

## **Workflow**

### Local Repository Structure

The local Git repository has three components:

1. Working Directory: The actual files reside here.
2. Index: The area used for staging
3. Head: Points to the most recent commit

![Workflow](https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)

### Saving Changes

All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

#### Tracked

Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

#### Untracked

Untracked files were not in the last snapshot and do not currently reside in the staging area.

*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

## **The Life Cycle of File Status**

1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
2. You stage the modified file.
3. Then, you commit staged changes.

![File-Status-Cycle](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

### Check File Status

To determine the state of files, utilize the git status command:

```
git status
```

### Tracking and Staging a New File

#### ***Single File***

Track one file only by using the following format:

```
git add filename
```

#### ***All Files***

Track all files in a repository by using the following command:

```
git add .
```

### Committing a File

After staging one or multiple files, you should commit the changes and record what you did within the commit message:

```
git commit -m “made change x,y,z”
```

This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

#### **Committing All Changes**

```
git commit -a
```

This command commits a snapshot of all modifications to tracked files in the working directory.

### Pushing Changes

Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

```
git push origin mmain
```

This command pushes changes from the local “main” branch to the remote repository named “origin”.

*For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.