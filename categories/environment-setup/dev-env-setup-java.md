## Development Environment Setup (Java)

- [JDK 8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea/download/index.html#section=mac)
- [Git](https://git-scm.com/downloads)
- [Maven](https://maven.apache.org/download.cgi)
- [MySQL](https://dev.mysql.com/downloads/mysql/)

## JDK Installation Instructions
When you install the Java Development Kit (JDK), the associated Java Runtime Environment (JRE) is installed at the same time. The JavaFX SDK and Runtime are also installed and integrated into the standard JDK directory structure.

Depending on your processor, the downloaded file has one of the following names:

`jdk-8uversion-macosx-amd64.dmg`

`jdk-8uversion-macosx-x64.dmg`

1. Download the file.

> Before the file can be downloaded, you must accept the license agreement.

2. From either the Downloads window of the browser, or from the file browser, double click the `.dmg` file to launch it.

> A Finder window appears containing an icon of an open box and the name of the `.pkg` file.

3. Double click the package icon to launch the Install app.

> The Install app displays the Introduction window.

4. Click **Continue**.

> The Installation Type window appears.

5. Click **Install**.

> A window appears that says "Installer is trying to install new software. Type your password to allow this."

6. Enter the Administrator login and password and click **Install Software**.

> The software is installed and a confirmation window appears.

7. Refer to [http://www.oracle.com/technetwork/java/javase/downloads/jdk-for-mac-readme-1564562.html](http://www.oracle.com/technetwork/java/javase/downloads/jdk-for-mac-readme-1564562.html) for more information about the installation.

8. After the software is installed, delete the `.dmg` file if you want to save disk space.

## Determining the Default Version of the JDK

You can determine which version of the JDK is the default by typing `java -version` in a Terminal window.

You should see something like the following:
```
java version "1.8.0_151"
Java(TM) SE Runtime Environment (build 1.8.0_151-b12)
Java HotSpot(TM) 64-Bit Server VM (build 25.151-b12, mixed mode)
```

## Download and install IntelliJ IDEA

IntelliJ IDEA is available in two editions: Ultimate and Community. The Community edition is an open-source project and is free, but it has less features. The Ultimate edition is commercial, and provides an outstanding set of tools and features.

To install IntelliJ IDEA Ultimate

1. Download IntelliJ IDEA Ultimate for your operating system. Here we are using macOS.

2. Double-click the ideaIC.dmg or ideaIU.dmg file you have downloaded to mount the macOS disk image.

3. Copy IntelliJ IDEA to the Applications folder.

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

## Install Maven on macOS

Mac OS X comes with Apache Maven 3 built in, and can be located at `/usr/share/maven`

## Maven Built-In

To verify the Maven installation, in terminal, issue the command `mvn -version`.

You should see something like the following:

```
Apache Maven 3.5.2 (138edd61fd100ec658bfa2d307c43b76940a5d7d; 2017-10-18T03:58:13-04:00)
Maven home: /usr/local/Cellar/maven/3.5.2/libexec
Java version: 1.8.0_151, vendor: Oracle Corporation
Java home: /Library/Java/JavaVirtualMachines/jdk1.8.0_151.jdk/Contents/Home/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "mac os x", version: "10.14.1", arch: "x86_64", family: "mac"
```

## Installing Maven on macOS Manually

To install Maven on Mac OS X operating system, download the latest version from the Apache [Maven](https://maven.apache.org/download.cgi) site, select the Maven binary tar.gz file, for example: apache-maven-3.6.0-bin.tar.gz.

Extract the archive to your desired location.

## Adding Maven to the Environment Path
Open the terminal and switch to the directory where the files were extracted to and then login as Super – User.

Remove the tar.gz archive:

```
rm Downloads/apache-maven*bin.tar.gz
```
Fix the permissions:
```
chown -R root:wheel Downloads/apache-maven*
```
Switch the Maven contents:
```
mv Downloads/apache-maven* /opt/apache-maven
```
Archive the Admin session:
```
exit
```
Add Maven binaries to the path and append.
```
nano $HOME/.profile
 
export PATH=$PATH:/opt/apache-maven/bin
```
Ctrl+x to Save and Exit from “nano”.

To load the new set up run:
```
bash
```
To test the new installation run:
```
mvn -version
```
You are now ready to use Maven on your Mac OS X.

## Installing MySQL on macOS

Oracle's MySQL is a popular open-source relational database management system that is based on Structured Query Language (SQL). It is frequently used in conjunction with PHP to enhance the capabilities of websites. PHP comes preloaded onto Mac computers, but MySQL does not.

When you create and test software or websites that require a MySQL database, it is handy to have MySQL installed on your computer. Installing MySQL on a Mac is easier than you might expect, particularly if you use the native installation package instead of the TAR package, which requires access and changes to the command line in Terminal mode.

## Installing MySQL Using the Native Installation Package

The free download for the Mac is the MySQL Community Server edition.

1. Go to the [MySQL website](https://dev.mysql.com/downloads/mysql/) and download the latest version of MySQL for MacOS. Select the native package DMG archive version, not the compressed TAR version.

2. Click the **Download** button next to the version you choose.

3. You are prompted to sign up for an Oracle Web Account, but unless you want one, click **No thanks, just start my download**.

4. In your downloads folder, find and double-click the **file icon** to mount the `.dmg` archive, which contains the installer.

5. Double-click the icon for the **MySQL package installer**.

6. Read the opening dialog screen and click **Continue** to begin the installation.

7. Read the license terms. Click **Continue** and then **Agree** to continue.

8. Click **Install**.

9. **Record the temporary password** that displays during the installation process. This password cannot be recovered. You must save it. After you log in to MySQL, you are prompted to create a new password.

10. Press **Close** on the Summary screen to complete the installation.

The MySQL webpage contains documentation, instructions and change history for the software. 

## How to Start My SQL on a Mac

The MySQL server is installed on the Mac, but it does not load by default. Start MySQL by clicking **Start** using the MySQL Preference Pane, which was installed during the default installation. You can configure MySQL to automatically start when you turn on your computer using the MySQL Preference Pane.
