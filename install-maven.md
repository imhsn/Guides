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
