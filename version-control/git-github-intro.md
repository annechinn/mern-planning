# Git Intro 1

### What is Version Control?

### Summary

_**Git**_ ****is a free and open source distributed version control system. Git is designed to work on a local repository. Internet access, or collaboration with other developers, is not required. The core functionality allows you to manage and keep track of your source code history on your local machine. Git does support sharing repositories with others across the internet, but at its core, its primary focus is source code control in a local repository.

Typically, within a development environment, collaboration is integral to the project, and there is a need to have a centralized location for the repository where developers share their repositories and can ensure automatic backups. This is where GitHub comes in.

_**GitHub**_ is a cloud-based hosting service that lets you store and manage Git repositories. It offers all of Git’s source code control functionality and additionally includes project management activities. GitHub is know for a place where the development community shares open source projects, but it is also where the vast majority of development teams host their company projects \(There are other similar services, such as Bitbucket\). With GitHub, developers can share their repositories, access other developers’ repositories, and store remote copies of repositories to serve as backups.

The following depicts the process that occurs on your local computer and the commands involved with working with your local repository, and the single push command that pushes the changes from your local repository to your corresponding GitHub repository.

![](../.gitbook/assets/image%20%28156%29.png)

### Using Git For Our Course

We'll going to start using Git/GitHub in a pretty simple use-case. We are going to ignore the concept of branching code and just work in the single main branch. We are also going to assume that you are the only developer working in your project. Branching and sharing a repository add complexity to Git and we're going to hold off on those tasks until we more fully understand the basics.

### Basic Git Usage to Start a New Project

Create your new project folder and create an index.html file \(need at least one file to add\).

#### Perform the following steps to create your local repository

* **git init** : initializes the folder as a Git repository
* **git add** --all : adds all of the files to the staging area 
* **git commit** -m"comment" commits the changes in the staging area to local repository.

![](../.gitbook/assets/image%20%2869%29.png)

#### Perform the following steps to push your local repository to GitHub

Log into GitHub and create a new repository. Accept all the defaults.

![](../.gitbook/assets/image%20%2854%29.png)

Follow the steps on the Quick Setup page for pushing an existing repository. 

![](../.gitbook/assets/image%20%28154%29.png)

![](../.gitbook/assets/image%20%2899%29.png)

Now you have created your local repository for you project, and updated the current version of it to a corresponding GitHub repository.

#### Updating the Local Repository and GitHub with New Versions

When you are at a point where you'd like to save the changes you've made as a unified new version, you use the following commands. 

The commit -am is a short-cut that combines git -add and git -commit into a single step, which in our simple use-case is fine.

It's a good practice to push these new local versions to GitHub each time you create a new version. All you have to do once that repository exists is the git push command.

So, you'll just repeat these two commands each time you want to create a new version of your project and push it to GitHub.

![](../.gitbook/assets/image%20%2860%29.png)

### Publishing your GitHub Repository to Netifly

Netifly allows you to easily publish your GitHub repository. 

* Signup with your GitHub account.
* On the Sites screen, click the New site from Git button
* On the Create a new site screen, click the GitHub button 
* On the next screen keep all the defaults and click the Deploy Site button at the bottom.
* Once the process completes, there should be an URL for the deployed site. 

Now you have a public website displaying your project.

### Additional Resources

This the best video I could find giving a good overview of Git/GitHub and how to get started.  It's very comprehensive, and may be a bit much to digest all at once. You can watch as much as you find useful to your understanding. The goal for now is to understand the general way Git and GitHub work together and how to create a local repository and get it pushed to GitHub. 

{% embed url="https://www.youtube.com/watch?v=xuB1Id2Wxak" %}

This one is shorter, and a bit more practical, gets to the point of the steps to get started.

{% embed url="https://www.youtube.com/watch?v=SWYqp7iY\_Tc" %}

