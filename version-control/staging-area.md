# Staging Area

### Review of Commits - Staging Area

One of the most confusing parts when you're first learning git is the concept of the staging environment and how it relates to a commit.

A commit is a record of what changes you have made since the last time you made a commit. Essentially, you make changes to your repo \(for example, adding a file or modifying one\) and then tell git to put those changes into a commit.

Commits make up the essence of your project and allow you to track the changes that have been made to the project over time. 

So, how do you tell git which files to put into a commit? This is where the staging environment or index come in.  When you make changes to your repo, git notices that a file has changed, but you must add new files to the staging area \(the set of files that will be included in the next commit\) for them to be included in the commit.

To add a file to a commit, you first need to add it to the staging environment. To do this, you can use the git add  command.

Once you've used the git add command to add all the files you want to the staging environment, you can then tell git to package them into a commit using the git commit command.

The image below outlines this process. 

* first you must create the local repository with "git init"
* next you iteratively add/commit changes to create a new "snapshot" of your work.
* optionally, you can push those snapshots to a repository on GitHub.

![](../.gitbook/assets/image%20%2830%29.png)



