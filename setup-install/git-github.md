# Version Control - Git/GitHub

### Setup for Using Git/GitHub

#### 1. Creating a GitHub Account

If you don't already have a GitHub account, go to the GitHub site and click the Sign-up button located at the upper right corner. Having a GitHub account will allow you to store/backup your local Git repositories on GitHub and also easily publish your completed projects using built-in integrations with the web hosting site Netlify.

{% embed url="https://github.com/" %}

#### 2. Install Git

{% embed url="https://git-scm.com/downloads" %}

#### 3. Set Global Configuration

During the installation process, some of these global settings might have the correct defaults. If you are having trouble when you attempt to push your local repository to GitHub, it may be because you don't have the user.name and user.email set correctly.

* git config --global user.name "your name"
* git config --global user.email "your email address"
* git config --global code.editor "code --wait"
* git config --global code.autocrlf true \(on Windows\)
* git config --global code.autocrlf input \(on Mac/Linux\)

{% hint style="info" %}
git config --global -e  will open the config file with your default editor and you can edit these directly.
{% endhint %}

#### 4. Change your default Terminal Shell to use Bash \(optional\)

* Ctrl-Shift-P to bring up the Command Palette.
* enter **Terminal: Select Default Profile**

