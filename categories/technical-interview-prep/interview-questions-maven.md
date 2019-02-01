Interview Questions -- Maven
===========================

**What is Maven?**

It is a software project management and comprehension tool.

**What are the Advantages of using Maven?**

It is used for projects build, dependency and documentation at the same time.

**What is the Life Cycle/Build Phases of Maven and outline/define all of them?**

```
validate - validate the project
compile  - compile the source code
test 	 - test the compiled source code
package  - take the compiled code and package it
verify 	 - run any checks on results
install  - install the package
deploy 	 - copies the final package to the remote repo
```

**What does the build tools do?**

Build tools are programs that automate the creation of executable applications from source code.

**What is the difference between Ant and Maven?**

There is no life cycle in Ant. But there is a life cycle in Maven.

**What is Archetype?**

Archetype is a Maven project templating toolkit. An archetype is defined as an original pattern or model from which all other things of the same kind are made.

**What is POM in Maven?**

A Project Object Model or POM is the fundamental unit of work in Maven.

**What is Repository in Maven and outline all of them?**

A repository in Maven is used to hold build artifacts and dependencies of varying types.

There are strictly only two types of repositories: local and remote.

**What is Dependency Management in Maven?**

The dependency management section is a mechanism for centralizing dependency information.

What is groupId, artifactId and version in Maven?

-   **groupId** identifies a project uniquely across all projects.
-   **artifactId** is the name of the jar without version.
-   **version** is if anyone distributes it, then they can choose any typical version with numbers and dots.
