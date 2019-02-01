## Setup Jenkins Pipeline

###### for Continuous Delivery Pipeline

## Install Pipeline plugin

Search plugin: *Pipeline*, if not installed, install it.

## Install Pipeline Maven Integration

Search plugin: *Pipeline Maven Integration*, install it.

## Create a new item as a Pipeline

Enter an item name and select Pipeline.

## Configure the item

Definition: Pipeline script from SCM

SCM: Git

Repositories: add repos url and credentials

Branches to build: specify the branch name

Repository browser: Auto

Script Path: jenkinsfile

Lightweight checkout: checked

## Add ‘Jenkinsfile’ to your project

```
pipeline {
    agent any
    stages {
        stage ('Compile Stage') {
            steps {
                withMaven(maven : 'Maven') {
                    sh 'mvn clean compile'
                }
            }
        }
        stage ('Testing Stage') {
            steps {
                withMaven(maven : 'Maven') {
                    sh 'mvn -fn test'
                }
            }
        }
    }
}
```

Push the changes to GitHub and build now from Jenkins.

## Resources

- [Jenkins Pipeline](https://jenkins.io/doc/book/pipeline/)
- [JenkinsFile Example](https://github.com/TechPrimers/jenkins-example/blob/master/Jenkinsfile)
- [Pipeline as Code with Jenkins](https://jenkins.io/solutions/pipeline/)
