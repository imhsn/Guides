### Setup Jenkins on AWS
Enable port 8081 on AWS

Goto AWS>EC2>security group>Inbound>Edit and add new role to port 8081.

### Installing Jenkins

```
$ wget -q -O - https://pkg.jenkins.io/debian/jenkins-ci.org.key | sudo apt-key add -
$ echo deb https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list
$ sudo apt-get update
$ sudo apt-get install jenkins
```

### Update Jenkins settings

```
$ sudo nano /etc/default/jenkins
change to “root”:	$JENKINS_USER="root"
replace to “8081”:	HTTP_PORT=8080 with HTTP_PORT=8081
```

Save the file.

Then change the ownership of the Jenkins home, Jenkins webroot and logs.

```
$ sudo chown -R root:root /var/lib/jenkins 
$ sudo chown -R root:root /var/cache/jenkins
$ sudo chown -R root:root /var/log/jenkins
```

### Start Jenkins

```
$ sudo /etc/init.d/jenkins start
$ ps -ef | grep jenkins
http://ip_address_or_domain_name:8081
$ sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```

### Global Tool Configuration

```
JDK home: /usr/lib/jvm/java-8-oracle/
Maven home: /usr/share/maven
```

### Install plugins

- Git client plugin
- Git plugin
- Git server Plugin
- GitHub API Plugin
- GitHub Branch Source Plugin
- GitHub Plugin

### Optional: if needed

### Starting Jenkins using systemctl

```
$ sudo systemctl start jenkins
$ sudo systemctl status jenkins
```

### Opening the Firewall

```
$ sudo ufw allow 8081
$ sudo ufw status
```

**Note:** If the firewall is inactive, the following commands will make sure that OpenSSH is allowed and then enable it.

```
$ sudo ufw allow OpenSSH
$ sudo ufw enable
```

### Install Google Chrome on Ubuntu 16.04

```
$ sudo nano /etc/apt/sources.list
```

### Add the following line:

```
deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main
```

### Save the file:

```
$ wget https://dl.google.com/linux/linux_signing_key.pub
$ sudo apt-key add linux_signing_key.pub
$ sudo apt update
$ sudo apt install google-chrome-stable
```

### Resources

- [Installing Jenkins on Linux [Debian/Ubuntu]](https://jenkins.io/doc/book/installing/#linux)
- [How To Install Jenkins on Ubuntu 16.04](https://www.digitalocean.com/community/tutorials/how-to-install-jenkins-on-ubuntu-16-04)
- [How to run Jenkins using the root user in Linux [CentOS]](https://medium.com/@farooqyousuf/how-to-run-jenkins-using-the-root-user-in-linux-centos-79d96749ca5a)
- [How to run Jenkins under a different user in Linux [Redhat]](http://blog.manula.org/2013/03/running-jenkins-under-different-user-in.html)
- [Two Ways to Install Google Chrome on Ubuntu 16.04 and Ubuntu 17.10](https://www.linuxbabe.com/ubuntu/install-google-chrome-ubuntu-16-04-lts)
