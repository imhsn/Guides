## Install Git on macOS

There are several ways to install Git on a Mac. In fact, if you've installed XCode (or it's Command Line Tools), Git may already be installed. 
To find out, open a terminal and enter `git --version`.

You should see something like the following:
```
git version 2.16.2
```

You may want to install a newer version of Git using one of the methods below:

## Git for Mac Installer

The easiest way to install Git on a Mac is via the stand-alone installer:

1. Download the latest [Git for Mac installer](https://sourceforge.net/projects/git-osx-installer/files/).

2. Follow the prompts to install Git.

3. Open a terminal and verify the installation was successful by typing `git --version`.

4. Configure your Git username and email using the following commands, replacing Emma's name and email with your own. These details will be associated with any commits that you create:

```
git config --global user.name "Emma Paris"
git config --global user.email "eparis@email.com"
```

## Install Git with Homebrew

If you have installed [Homebrew](http://brew.sh/) to manage packages on OS X, you can follow these instructions to install Git:

1. Open your terminal and install Git using Homebrew:

```
brew install git
```

2. Verify the installation was successful by typing which `git --version`.

3. Configure your Git username and email using the following commands, replacing Emma's name and email with your own. These details will be associated with any commits that you create:

```
git config --global user.name "Emma Paris"
git config --global user.email "eparis@email.com"
```
