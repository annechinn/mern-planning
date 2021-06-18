# Git Intro 2

### Creating/Connecting to GitHub Repositories

#### Case 1 - You started a local repository first, worked on it for awhile, and now you want to also store the repository on GitHub  \(no collaboration\)

In this scenario, you will have initialized a local repository with "git init", and used the local git commands to track changes to your code by adding/committing files within your local repository. Then you decide you want to push your local repository to GitHub.

In this scenario you just need to create a repository in GitHub, connect it to your local repository, and push the files from the local repository to the GitHub repository.

The "git remote add origin \[gitHub repository url\]" is connecting the local repository with the GitHub repository. The term "origin" is telling git what to call the remote GitHub repository. You could use any label you want, but "origin" is the convention. This label is necessary so that future commands, such as "push origin", can tell git what remote GitHub repository the command is targeting.

The second command "git branch -M main" is necessary because git historically named the default branch "master" and about six months ago, they decided to change the default branch name to "main". 

![](../.gitbook/assets/image%20%283%29.png)

* **git remote add origin \[GitHubURL\]**: connects to the local repository with the GitHub Repository
* **git branch -M main:** changes the default "master" branch to "main"
* **git push -u origin main**: pushes all the files in your local repository to the GitHub repository. 

Below is a history of the steps required to first create a local repository, make some edits, and then create and connect to a GitHub repository.

![](../.gitbook/assets/image%20%28136%29.png)

#### Case 2 - You want to start a new project and it will also be on GitHub \(no collaboration\)

In this scenario, you can create either the local repository or the GitHub repository first. In either case, you need get the default branch created, and this requires committing at least one file. 

#### Starting with a local repository

If you start with the local repository first, then you can follow these steps to initialize the local repository with a single file \(they create the standard README.md file\), commit the changes, and then connect the local repository to the GitHub repository. This is pretty much following the previous case, where you created a local repository and then decided to create a GitHub repository to push it to. 

The key is that you need to commit a single file to initialize the local repository, and once that happens, you can rename the "master" branch to "main" and then connect the local repository to the GitHub repository and push your local repository to the GitHub repository.

![](../.gitbook/assets/image%20%2849%29.png)

#### Starting with GitHub repository 

If you create the GitHub repository first, then you can create the initial file within GitHub and it will be created on the "main" branch by default. This eliminates the need to perform all of the steps below, which are just creating that initial file and the main branch on the command line.

![](../.gitbook/assets/image%20%2843%29.png)

Instead, create the repository in GitHub...

![](../.gitbook/assets/image%20%28129%29.png)

And then create a new file within GitHub. Creating the file within the new GitHub repository is performing all of the steps in the first "...or create a new repository on the command line". So we're all done at this point. The repository is set up.

![](../.gitbook/assets/image%20%2885%29.png)

 At this point you have a repository on GitHub that is equivalent to any repository that is hosted there and you can use "git clone" to create a local repository that is connected to the GitHub repository. 

#### Case 3 - Cloning a GitHub Repository

Cloning is how you download a copy of an existing GitHub repository and associate your local repository to the GitHub repository. It may be a repository that you created for private use or a repository that contains the sources for a product at your company and you need to connect to it.

In either case, you can clone a GitHub repository, which downloads the repository to your local computer and initializes it so that there is a connection between the GitHub repository and your local repository.

Once you clone the repository, you can immediately start working in the local repository and the connection with the GitHub repository already exists. 

The process of cloning the repository performs the command "git add remote origin \[GitHub repo Url\]" behind the scenes. So you can do "git push", and git will know that you are pushing to "origin".

To clone a repository, you go to the Code page, click the Code button and click the clipboard icon next to the GitHub repository URL.

![](../.gitbook/assets/image%20%28137%29.png)

On your local computer, go to the directory where you want to setup the local repository and from the command line type "git clone \[the url copied above\]". This will pull all of the files from the repository to a local repository with the same name. After this command, you have all the setup necessary to start working in the local repository.

![](../.gitbook/assets/image%20%28166%29.png)

![](../.gitbook/assets/image%20%2876%29.png)

#### Case 4 - Forking a GitHub Repository

You fork a repository when you want to create a copy of someone else's repository in your own GitHub account. There are two use-cases for forking a GitHub repository.

* want to have a private copy of a repository from someone else's account.
* want to contribute to an open-source project.

Once you have forked the repository, it exists in your GitHub account, but does not yet exist on your local computer as a local repository. To do that you would just clone the repository.

We'll defer the process of contributing to an open source project for now and just use fork as a way to copy a repository from my GitHub account to start a private copy in your own GitHub account.

{% embed url="https://levelup.gitconnected.com/how-to-sync-forked-repositories-using-git-or-github-2933e497fa16" %}



Watch this video to review the different options for how to create a repository. The only caveat is that  it was created before the rename of "master" to "main" happened, so they have the "master" branch as the default branch.

{% embed url="https://www.youtube.com/watch?v=fQLK8Ib\_SKk&t=756s" %}

