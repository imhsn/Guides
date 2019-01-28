# Install Maven on Windows 10

At first, make sure **JDK** is installed and `JAVA_HOME` environment variable is configured properly.

# Download

Download the Maven zip file from [here](https://maven.apache.org/download.cgi). 

`Example: apache-maven-3.6.0-bin.zip`

Unzip it to a folder. 

`Example: C:\Maven\apache-maven-3.6.0` 

# Setup MAVEN_HOME

Search for **Advanced System Settings** from your desktop search box.

Click on **Environment Variables**.

Click on **New** button under System variables to create *MAVEN_HOME*.

Enter variable name as `MAVEN_HOME`, variable value as your *Maven path* and click **OK**. 

`[ Maven path example: C:\Maven\apache-maven-3.6.0 ]` 

Select **Path variable** and click on **Edit** button.

Click on **New** button and add environment variable `%MAVEN_HOME%\bin` .

Click on **OK**.

Now your setup is done.

You can check it by opening a command prompt and running the following command:

`mvn -version`

You will see the result as following:

```
Apache Maven 3.6.0 (97c98ec64a1fdfee7767ce5ffb20918da4f719f3; 2018-10-24T14:41:47-04:00)
Maven home: C:\Maven\apache-maven-3.6.0\bin\..
Java version: 1.8.0_192, vendor: Oracle Corporation, runtime: C:\Program Files\Java\jdk1.8.0_192\jre
Default locale: en_US, platform encoding: Cp1252
OS name: "windows 10", version: "10.0", arch: "amd64", family: "windows"
```
